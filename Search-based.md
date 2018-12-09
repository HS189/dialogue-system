refer:<br>[智能客服FAQ问答任务的技术选型探讨](https://zhuanlan.zhihu.com/p/50799128)<br>[问题对语义相似度计算-参赛总结](http://www.zhuzongkui.top/2018/08/10/competition-summary/)





蚂蚁金服:

![智能客服](https://github.com/bifeng/dialogue-system/raw/master/image/qa_ant_finance.png)



#### 方案设计

1. 规则+模型

   规则：

   关键词匹配，主要保证准确率

   模型：

   语义匹配，主要提高问题的召回率（Q-Q paris 语义匹配的精度不高，所以也只适用于召回场景）

2. 模型

   排序（Learning to rank）



#### 数据标注

方法一，前期用规则方法，待数据积累到一定量级，从日志中抽取用户的输入，然后粗略用一些规则和聚类算法，然后把每个类的对应question列表，两两组合去生成样本，然后人工来标注

方法二，Paraphrase Generation

方法三，人工编写相似问法

方法一 避免脑补的相似问法；方法二 如何保证相似问法的多样性，而不仅仅是关键词的排列组合？方法三 不是真实的相似问法，且各标注人员的业务理解存在差异

Q-Q paris构建及建模的注意事项：

1. 数据增强

   假设 Q1 在所有样本里出现2次，分别是

   label, question, question

   1，Q1，Q2
   1，Q3，Q1
   模型无法正确学习Q1与Q2/Q3的相同，而是会认为只要input里有Q1即为正样本。
   需要通过数据处理引导模型进行“比较”，而不是“拟合”。
   解决方案：通过构建一部分补充集（负例），对冲所有不平衡的问题。

2. 后处理

   - 传递关系

     相似：（AB=1，AC=1）—> BC=1

     不相似：（AB=1，AC=0）—> BC=0

   - infer机制

     除了判断test集的每个样本得分以外，还会通过已知同义问题集的其他样本比对进行加权；融合时轻微降低得分过高的模型权重，补偿正样本过多的影响；将已知确认的样本修正为0/1。



+ 为什么问答检索场景，选择Q-Q pairs相似性建模，而不是Q-A pairs相似性建模？

1. 支持业务需求变更

   Q-Q paris建模，相当于将问题与答案的解耦，只需要关注于问题，当业务发生变更时，只需更新相关问题的答案，无需重新训练模型！

2. Question Understanding/Representation

   Q-Q paris建模，相当于一个NLU引擎，对于问题都能获得一个很好的表示，有利于语料更新及模型迭代。如通过语义聚类，发现新问题与重复问题去重。

3. 迁移学习

   预训练一个开放域的Q-Q pars 语义匹配模型，再在垂直域进行fine-tuning！



#### QA

**Q:** The cosine similarity of two sentence vectors is unreasonably high (e.g. always > 0.8), what's wrong?

(This question is from [bert as service](https://github.com/hanxiao/bert-as-service).)

**A:** A decent representation for a downstream task doesn't mean that it will be meaningful in terms of cosine distance. Since cosine distance is a linear space where all dimensions are weighted equally. if you want to use cosine distance anyway, then please focus on the rank not the absolute value. Namely, do not use:

```
if cosine(A, B) > 0.9, then A and B are similar
```

Please consider the following instead:

```
if cosine(A, B) > cosine(A, C), then A is more similar to B than C.
```



