#### key phrases

- architecture, difficulty

#### Progress

目前 KBQA 主要应用于简单的知识库问答，无法进行复杂的推理等。

#### Architecture

+ semi-supervised / unsupervised

+ supervised method

  + pipeline - 问题理解分为两个步骤：实体识别、属性抽取。将问题中提取的实体及属性作为知识库的查询。

    **question understanding**

    1. **Entity**

    - entity recognize

      时间、数字、人名、地名等实体

      规则方法

      序列标注方法

    - entity disambiguation

      knowledge graph/context/user portrait

    2. **Relation**

       shallow parser

    - relation extractive (subject 、predicate、object)
    - semantic role labeling (SRL, predicate、argument）, , SRL is figure out who did what do whom. 

  + end2end - 直接学习问题到查询的映射。


#### Difficulty

当前难点在于：

1. 如何将用户问题转化为数据库查询？
2. 如何构建知识图谱？实体对齐、知识融合等
3. 如何评测？

工程上，从简单的实体关系入手。首先定义知识图谱的**边界**，即图谱中包含哪些类型的实体、实体之间包括哪些层次关系，其次...。

#### Application

+ 大规模医疗知识图谱的构建与应用, 2018 刘升平博士，资深技术专家，云知声 AI Labs [ppt](http://www.ccks2018.cn/)
+ 《大词林》中实体上位词获取及层次化构建方法, 2015 - [ppt](http://qngw2014.bj.bcebos.com/upload/kg3/KG%202015%20-%E3%80%8A%E5%A4%A7%E8%AF%8D%E6%9E%97%E3%80%8B%E4%B8%AD%E5%AE%9E%E4%BD%93%E4%B8%8A%E4%BD%8D%E8%AF%8D%E8%8E%B7%E5%8F%96%E5%8F%8A%E5%B1%82%E6%AC%A1%E5%8C%96%E6%9E%84%E5%BB%BA%E6%96%B9%E6%B3%95.pdf) 
+ 

#### Question

+ query 实体消歧

  query中的实体不在知识库中，但知识库存在该实体的同义词？

  query查询获得多个结果，且实体的具体含义各不相同？（反问用户，获取信息）

+ 知识库 实体消歧 - 知识库存在多个同义实体？




