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

当前难点在于如何将用户问题转化为数据库查询？

工程上，从简单的实体关系入手。首先定义知识图谱的**边界**，即图谱中包含哪些类型的实体、实体之间包括哪些关系，其次...。



#### Question

+ query 实体消歧

  query中的实体不在知识库中，但知识库存在该实体的同义词？

  query查询获得多个结果，且实体的具体含义各不相同？（反问用户，获取信息）

+ 知识库 实体消歧 - 知识库存在多个同义实体？




