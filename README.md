## dialogue-system

## Methods

### dependency parsing

## Challenges

### multi-hop

### dialogue management  (context)

#### 多场景切换

#### 跨场景继承

#### Retrieval Based

#### Knowledge Based

### natural language understanding

#### personality (人格)

如何让机器人具有特定的说话风格

#### sentimental (情商)

#### semantic phenomena

##### coreference

https://medium.com/huggingface/state-of-the-art-neural-coreference-resolution-for-chatbots-3302365dcf30

##### anaphora

##### ellipsis

#### utterance compression

### natural language generation

#### sentence editing (句子可控改写)

#### grammar error detection

## Competition

+ NLPCC

  NLPCC 2017

  http://tcci.ccf.org.cn/conference/2017/taskdata.php

  + Emotional Conversation Generation

    http://coai.cs.tsinghua.edu.cn/hml/challenge/

    [Overview of the NLPCC 2017 Shared Task: Emotion Generation Challenge](http://coai.cs.tsinghua.edu.cn/hml/media/files/Overview_of_the_NLPCC_2017_Shared_Task__Emotion_Generation_Challenge.pdf)

    [Second - Babbling-The HIT-SCIR System for Emotional Conversation Generation]()

  NLPCC 2018

  http://tcci.ccf.org.cn/conference/2018/taskdata.php


---

STC (Short Text Conversation)

http://ntcirstc.noahlab.com.hk/STC2/stc-cn.htm

## Paper

### 2019

+ Response Generation by Context-aware Prototype Editing AAAI-19 [arxiv](https://arxiv.org/abs/1806.07042) | [code](https://github.com/MarkWuNLP/ResponseEdit)
  + [x] sentence editing

  ???

+ Learning Personalized End-to-End Goal-Oriented Dialog AAAI-19 [arxiv](https://arxiv.org/abs/1811.04604)

  - [x] personalized

  ???


### 2018

+ [Deep Learning for Dialogue Systems](http://deepdialogue.miulab.tw/) COLING

  ？？？


- A Survey on Dialogue Systems: Recent Advances and New Frontiers JD [arxiv](https://arxiv.org/abs/1711.01731)

  ???

- Emotional Chatting Machine: Emotional Conversation Generation with Internal and External Memory AAAI 2018 [arxiv](https://arxiv.org/abs/1704.01074) | [data](http://coai.cs.tsinghua.edu.cn/hml/dataset/)

  - [x] natural language generation
  - [x] sentimental

  ???

- Commonsense for Generative Multi-Hop Question Answering Tasks EMNLP [arxiv](https://export.arxiv.org/abs/1809.06309) | [code](https://github.com/yicheng-w/CommonSenseMultiHopQA)

  - [x] multi-hop

  ???

- Building an Ellipsis-aware Chinese Dependency Treebank for Web Text [arxiv](https://arxiv.org/abs/1801.06613) | [code](https://github.com/lancopku/Chinese-Dependency-Treebank-with-Ellipsis)

  - [x] ellipses 

- Assigning personality/identity to a chatting machine for coherent conversation generation, IJCAI 2018 [arxiv](https://arxiv.org/abs/1706.02861) | [code](https://github.com/qianqiao/AssignPersonality) | [data](http://coai.cs.tsinghua.edu.cn/hml/dataset/)

  - [x] personality

    personality, includes name, gender, age, location, weight, constellation, hobby, idol, speciality, employer - extracted from Weibo Dataset with regular expression patterns.

    为了可控性，可以直接用正则表达式解决！

  ???

---

### 2017

+ Teaching Machines to Converse [code](https://github.com/jiweil/Jiwei-Thesis)

  ???

+ Sequential Matching Network: A New Architecture for Multi-turn Response Selection in Retrieval-based Chatbots. ACL. 2017 [code](https://github.com/MarkWuNLP/MultiTurnResponseSelection)

  - [x] Retrieval Based

  ???

+ Question Answering on Knowledge Bases and Text using Universal Schema and Memory Networks ACL 2017 [arxiv](https://arxiv.org/abs/1704.08384) | [code](https://github.com/rajarshd/TextKBQA)

  - [x] Knowledge Based

  ???

---





### 2015

+ Ground Truth for Grammatical Error Correction Metrics  ACL 2015 [code](https://github.com/cnap/gec-ranking)

  - [x] grammar error detection

  ???



---

### 2012

+ A Two-step Approach to Sentence Compression of Spoken Utterances ACL 2012 [paper](http://aclweb.org/anthology//P/P12/P12-2033.pdf)
  + [x] utterance compression

  ???



---

### 2010

+ Using spoken utterance compression for meeting summarization: a pilot study, SLT 2010 [paper]()

  - [x] utterance compression

  ???



---



### 2005

+ Question Answering Passage Retrieval Using Dependency Relations. [paper](https://www.comp.nus.edu.sg/~kanmy/papers/f66-cui.pdf) | [slides](https://www.comp.nus.edu.sg/~kanmy/papers/deppass_draft_v0.5.htm)
  - [x] dependency parsing



---





more refer:

实录分享 | 计算未来轻沙龙：对话系统研究进展（视频 + PPT）

https://blog.csdn.net/c9Yv2cf9I06K2A9E/article/details/82392595

CIIS2018演讲实录丨哈尔滨工业大学车万翔：任务型对话系统研究进展

https://mp.weixin.qq.com/s/UZbt1E6QntwtWWvJfTL3eQ

???

https://github.com/bnsblue/awesome-dialogue-management

[多轮对话之对话管理(Dialog Management)](https://zhuanlan.zhihu.com/p/32716205)

**1. aiml 地址**

https://github.com/Shuang0420/aiml

**2. 填槽与多轮对话**

http://t.cn/RQfkTPP

**3. CMU Communicator 论文**

http://www.cs.cmu.edu/~xw/asru99-agenda.pdf

**4. NLP 笔记 - Meaning Representation Languages**

http://t.cn/RQfFMAo

**5. NLP 笔记 - Discourse Analysis**

http://t.cn/RQfFacE

**6. Plan-based models of dialogue**

http://t.cn/RQfFC1b





