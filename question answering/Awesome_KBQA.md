## Challenge

+ single relation
+ multiple relation



## Knowledge Base

知识库通常由大量的三元组组成，每一条三元组包括：entity - relation - entity，如果我们把实体看作是结点，把实体关系（包括属性，类别等等）看作是一条边，那么包含了大量三元组的知识库就成为了一个庞大的知识图。



Freebase 



## Dataset

+ WebQuestion

  Stanford在2013年的论文 Semantic Parsing on Freebase from Question-Answer Pairs 中提出，其中包含了5,810 条问答对。

+ SimpleQuestion

  Facebook在2015年的论文 Large-scale Simple Question Answering with Memory Networks 中开放，包含了10w多条问答对，但是只包括简单问题：由一条三元组就可以回答的问题，也叫single-relation问题。





## Scholars

- 刘焕勇 [github](<https://github.com/liuhuanyong>) 





## Competition

+ CCKS 2018

  <https://github.com/songlei1994/ccks2018>

+ NLPCC 2016 KBQA

  <https://github.com/huangxiangzhou/NLPCC2016KBQA>

  基于知识图谱的问答系统入门之—NLPCC2016KBQA数据集 [site](<https://zhuanlan.zhihu.com/p/53796189?edition=yidianzixun&utm_source=yidianzixun&yidian_docid=0L0P0oIV>) 

+ 





## Case

+ 医药知识图谱

  https://github.com/liuhuanyong/QASystemOnMedicalKG star1.5k :star::star::star::star:

  <https://github.com/zhihao-chen/QASystemOnMedicalGraph>

+ 医疗对话系统

  <https://github.com/baiyang2464/chatbot-base-on-Knowledge-Graph>

+ [证券知识图谱](https://github.com/lemonhu/stock-knowledge-graph) star 585

+ [电影知识图谱](https://github.com/SimmerChan/KG-demo-for-movie) star 599

+ 电影知识图谱 [blog](<https://blog.csdn.net/appleyk/article/details/80422055>) [code](<https://github.com/kobeyk/Spring-Boot-Neo4j-Movies>) star 166

+ [中文百科类知识图谱](https://github.com/Pelhans/Z_knowledge_graph) star 395

+ 王昊奋老师发布在OpenKG上的demo [基于 REfO 的 KBQA 实现及示例](http://openkg.cn/tool/refo-kbqa) :star::star::star:

  > 1. 本文代码中对自然语言问句进行正则匹配的逻辑兼容 REfO. 主要参考代码为:
  >    https://github.com/machinalis/refo/blob/master/examples/words.py
  >
  > 2. 本文代码的后续改进可参考: https://github.com/machinalis/quepy
  > ● 使用邻接链表表示自然语言问句
  > ● 通过遍历有向图或子图匹配方法构造 SPAPQL 查询语句

+ gAnswer

  <http://openkg.cn/tool/ganswer>

  > 一个基于开放领域知识图谱的自然语言问答(QA)系统，能够将自然语言问题转化成包含语义信息的查询图，并将查询图转化成标准的SPARQL查询，将这些查询在图数据库(gStore)中执行，最终得到用户的答案。目前英文问答基于DBpedia2016数据集，中文问答基于PKU BASE。

+ 基于知识图谱的问答系统(KBQA) [site](<https://blog.csdn.net/keyue123/article/details/85266355>) 

+ 基于ElasticSearch的问答系统(KBQA) [site](<https://blog.csdn.net/keyue123/article/details/85317774>) 

+ 基于知识库的问答：seq2seq模型实践 <https://github.com/wavewangyue/kbqa>





## Blogs

+ 知识图谱入门 (九)

  http://pelhans.com/2018/04/28/xiaoxiangkg-note9/#模板定义
  
+ 揭开知识库问答KB-QA的面纱0·导读篇

  <https://zhuanlan.zhihu.com/p/27141786>
  
+ 自由讨论 | KBQA从入门到放弃—入门篇

  http://blog.openkg.cn/自由讨论-kbqa从入门到放弃-入门篇/







## STOA

+ <https://paperswithcode.com/task/knowledge-base-question-answering>
+ <http://nlpprogress.com/english/question_answering.html#knowledge-base-question-answering>
+ 



## Literature Review

+ Core Techniques of Question Answering Systems over Knowledge Bases: a Survey
  Dennis Diefenbach, Vanessa Lopez, Kamal Singh and Pierre Maret, 2017 KAIS [paper](<http://wdaqua.eu/assets/publications/2017_KAIS.pdf>) 

+ 
  
+ 
  
+ 
  
+ 
  
+ KBQA 知识库问答领域研究综述（未完待续。。）[site](<https://blog.csdn.net/u012892939/article/details/79451978>) 
  


## Paper

+ 

+ single relation

  

+ multiple relation

  Wen-tau Yih, Ming-Wei Chang, Xiaodong He, and Jianfeng Gao. 2015. Semantic parsing via staged query graph generation: Question answering with knowledge base.

  KBQA: Learning Question Answering over QA Corpora and Knowledge Bases. [paper](<http://www.vldb.org/pvldb/vol10/p565-cui.pdf>) 











