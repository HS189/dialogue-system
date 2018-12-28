Question:

How to make dialogue system more human?



#### human characteristic

[robot infor](https://github.com/bifeng/dialogue-system/raw/master/branch/robot_infor.md)

user infor



#### question understanding

##### Entity

+ entity recognize

  时间、数字、人名、地名等实体

  规则方法

  序列标注方法

+ entity disambiguation

  knowledge graph/context/user portrait

##### Relation

shallow parser

+ relation extractive (subject 、predicate、object)
+ semantic role labeling (SRL, predicate、argument）, , SRL is figure out who did what do whom. 



#### dialogue management (context)

1，上下文
当前语义

上下文语义


2，理解

规则方法
方法一
槽作为语义变量，其余成分作为辅助信息
示例：

```
{time}{city}天气怎么样？
```

方法二
将句子看成不同成分或语义变量的组合
示例：

```
[time][city][weather]([how]|)
```

`[]` 表示必选
`(|)`表示可选

比较：
与方法一相比，方法二只需穷举句式规则，并且语义变量可为其他句式共享。
不过需要注意的是，槽周围的语义变量应为必选内容，可以避免句式规则之间的冲突。

方法二需要人工穷举的地方：
1. 槽等语义变量的词表（值）
  （可选语义变量可有可无，所以无需穷举）
2. 槽的组合句式。n个槽，就需要有2^n个句式才能完整覆盖
3. 句式规则。即使两个句式使用相同的槽，句式规则也不一样