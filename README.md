dialogue-system

## Methods

### linguistically/semantically

#### dependency parsing

### neural networks

## Challenges

### multi-hop

### dialogue management  (context)

#### 多场景切换

#### 跨场景继承

### natural language understanding

#### personality (人格)

如何让机器人具有特定的说话风格

#### sentimental (情商)

#### semantic phenomena

##### coreference

https://medium.com/huggingface/state-of-the-art-neural-coreference-resolution-for-chatbots-3302365dcf30

##### anaphora/pronoun resolution

##### ellipsis

##### sentence function 

interrogative, declarative, imperative, and exclamatory

#### utterance compression

#### short text understanding

### natural language generation

#### sentence editing (句子可控改写)

#### grammar error detection

### data augmentation



## Application

### 微软 小冰

- The Design and Implementation of XiaoIce, an Empathetic Social Chatbot, [arxiv](https://arxiv.org/pdf/1812.08989.pdf)

  详细介绍了系统架构和关键组件，包括对话管理器、核心聊天、技能和移情计算模块。在系统设计中考虑了智商（IQ）和情商（EQ），将人机社交聊天作为马尔可夫决策过程（MDP）的决策，并优化了小冰的长期用户参与度和预期的每次会话对话（CPS）。我们展示了小冰如何动态识别人类的感受和状态，理解用户意图，并在长时间的对话中响应用户需求。

- From Eliza to XiaoIce: Challenges and Opportunities with Social Chatbots, [arxiv](https://arxiv.org/abs/1801.01957)

- 全双工语音对话以及在智能硬件上的应用，微软小冰全球首席架构师及研发总监周力，2019.01.17

- 微软小冰与情感计算框架，微软（亚洲）互联网工程院副院长李笛，2019.01.10 [ppt and video](https://pan.baidu.com/s/1jTM0J9kqnG_Jl1cfsAUdMA)

- 微软小冰技术交流会，微软（亚洲）互联网工程院，2018.03.28

  全双工语音交互感官（Full-duplex Voice Sense）

- 研发人员

  微软小冰首席科学家武威 [publications](https://www.microsoft.com/en-us/research/people/wuwei/#!publications)

  微软小冰全球首席架构师及研发总监周力

### Alex

+ Alex Dialogue Systems Framework [github](https://github.com/UFAL-DSG/alex)


### AliMe

+ AliMe Assist: An Intelligent Assistant for Creating an Innovative E-commerce Experience, 2018 [arxiv](https://arxiv.org/abs/1801.05032)

+ AliMe Chat: A Sequence to Sequence and Rerank based Chatbot Engine, ACL 2017 [paper](http://aclweb.org/anthology/P17-2079)


### Replika.ai

+ CakeChat: Emotional Generative Dialog System [https://cakechat.replika.ai](https://cakechat.replika.ai/) | [code](https://github.com/lukalabs/cakechat)

### SenticNet

+ https://github.com/SenticNet



## Challenge

+ SLT 2018 Special Session - Microsoft Dialogue Challenge: Building End-to-End Task-Completion Dialogue Systems

  https://github.com/xiul-msr/e2e_dialog_challenge

+ 2017 NIPS Conversational Intelligence Challenge 

  [1st place](https://github.com/sld/convai-bot-1337)

## Competition

+ NLPCC

  NLPCC 2016

  + Open Domain Question Answering System Based on Knowledge Base

    1st [code](https://github.com/huangxiangzhou/NLPCC2016KBQA)

  NLPCC 2017

  http://tcci.ccf.org.cn/conference/2017/taskdata.php

  http://tcci.ccf.org.cn/conference/2017/papers/

  + **Emotional Conversation Generation**

    http://coai.cs.tsinghua.edu.cn/hml/challenge/

    Overview of the NLPCC 2017 Shared Task: Emotion Generation Challenge [paper](http://coai.cs.tsinghua.edu.cn/hml/media/files/Overview_of_the_NLPCC_2017_Shared_Task__Emotion_Generation_Challenge.pdf)

    [Second - Babbling-The HIT-SCIR System for Emotional Conversation Generation]()

  NLPCC 2018

  http://tcci.ccf.org.cn/conference/2018/taskdata.php

  http://tcci.ccf.org.cn/conference/2018/papers/

  + **Grammatical Error Correction**

  + **Spoken Language Understanding in Task-Oriented Dialogue Systems**

    Overview of the NLPCC 2018 Shared Task: Spoken Language Understanding in Task-Oriented Dialog Systems, [paper](tcci.ccf.org.cn/conference/**2018**/papers/EV33.pdf)

  + **Multi-Turn Human-Computer Conversations**

    Overview of the NLPCC 2018 Shared Task: Multi-turn Human-Computer
    Conversations [paper](http://tcci.ccf.org.cn/conference/2018/papers/EV52.pdf)

    1st [paper](http://tcci.ccf.org.cn/conference/2018/papers/EV43.pdf)

    2nd [paper](http://tcci.ccf.org.cn/conference/2018/papers/EV5.pdf) | [code](https://github.com/jimth001/NLPCC2018_Multi_Turn_Response_Selection)

  + **Open Domain Question Answering**

    Overview of the NLPCC 2018 Shared Task: Open Domain QA [paper](http://tcci.ccf.org.cn/conference/2018/papers/EV51.pdf)

---

+ STC (Short Text Conversation)

  [NTCIR-12](http://research.nii.ac.jp/ntcir/ntcir-12/index.html) - October 31, 2015

  +  [STC](http://ntcir12.noahlab.com.hk/stc.htm)
  + Single-round, chatbot
  + retrieval
  + Overview of the NTCIR-12 Short Text Conversation Task, [paper](http://research.nii.ac.jp/ntcir/workshop/OnlineProceedings12/pdf/ntcir/OVERVIEW/01-NTCIR12-OV-STC-ShangL.pdf) | [slides](http://research.nii.ac.jp/ntcir/workshop/OnlineProceedings12/pdf/ntcir/OVERVIEW/01-NTCIR12-OV-STC-ShangL_slides.pdf)

  [NTCIR-13](http://research.nii.ac.jp/ntcir/ntcir-13/index.html) - April 30th 2017

  + [STC-2](http://ntcirstc.noahlab.com.hk/STC2/stc-cn.htm)
  + Single-round, chatbot
  + retrieval, generation
  + Overview of the NTCIR-13 Short Text Conversation Task, [paper](http://research.nii.ac.jp/ntcir/workshop/OnlineProceedings13/pdf/ntcir/01-NTCIR13-OV-STC-ShangL.pdf)
  + 1st, SG01 at the NTCIR-13 STC-2 Task [paper](https://pdfs.semanticscholar.org/27db/6405eb83709918d75b87fe80ba5acc36277f.pdf)

  [NTCIR-14](http://research.nii.ac.jp/ntcir/ntcir-14/index.html) - Sep 9th, 2018

  + [STC-3](http://sakailab.com/ntcir14stc3/)

  + Chinese Emotional Conversation Generation subtask, [datasets](http://coai.cs.tsinghua.edu.cn/hml/challenge/dataset_description/)

    Single-round, chatbot

  + Dialogue Quality subtask

    Multi-round, task-oriented chatbot

  + Nugget Detection subtask

    Multi-round, task-oriented chatbot


## Literature review

### 2018

+ Deep Chit-Chat: Deep Learning for ChatBots, Wei Wu and Rui Yan, EMNLP [ppt](http://www.ruiyan.me/pubs/tutorial-emnlp18.pdf) | [video](https://vimeo.com/305179403)

  微软小冰首席科学家武威

  北京大学助理教授严睿

+ Neural Approaches to Conversational AI, Jianfeng Gao, [arxiv](https://arxiv.org/abs/1809.08267)

  Neural Approaches to Conversational AI ACL 2018 [ppt](https://www.microsoft.com/en-us/research/uploads/prod/2018/07/neural-approaches-to-conversational-AI.pdf) 

- A Survey on Dialogue Systems: Recent Advances and New Frontiers, JD [arxiv](https://arxiv.org/abs/1711.01731)

- Deep Learning for Dialogue Systems, COLING [site](http://deepdialogue.miulab.tw/) 

### 2017

+ Teaching Machines to Converse, Jiwei Li's Thesis 2017 [code](https://github.com/jiweil/Jiwei-Thesis) | [thesis](https://github.com/jiweil/Jiwei-Thesis/blob/master/thesis.pdf)


### Question

+ Neural approaches in spoken language understanding is just for domain or intent detection and slot filling?

## Paper list

Neural Network Dialog System Papers [github](https://github.com/snakeztc/NeuralDialogPapers) active

deeplearning-papernotes [github](https://github.com/sld/deeplearning-papernotes) active

chatbots [github](https://github.com/minghui/chatbots) - product attention, such as AliMe!!!

chatbots [github](https://github.com/fuzhenxin/Personal-Emotional-Stylized-Dialog) - personalized, emotional, and stylized  attention!!!

chatbots [github](https://github.com/IsaacChanghau/DL-NLP-Readings/blob/master/readme/nlp/dialogue.md) - 2018

chatbots [github](https://github.com/ricsinaruto/Seq2seqChatbots/wiki/Chatbot-and-Related-Research-Paper-Notes-with-Images) - 2017

## Paper

### 2019

+ Learning Personalized End-to-End Goal-Oriented Dialog AAAI-19 [arxiv](https://arxiv.org/abs/1811.04604)

  - [x] personalized

  ???


### 2018


- Emotional Chatting Machine: Emotional Conversation Generation with Internal and External Memory AAAI 2018 [arxiv](https://arxiv.org/abs/1704.01074) | [data](http://coai.cs.tsinghua.edu.cn/hml/dataset/) | [code](http://coai.cs.tsinghua.edu.cn/publications/)

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

- Generating Informative Responses with Controlled Sentence Function. ACL 2018 [paper](http://aclweb.org/anthology/P18-1139) | [data](http://coai.cs.tsinghua.edu.cn/hml/dataset/) | [code](https://github.com/kepei1106/SentenceFunction)

  - [x]  sentence function


  - [x] natural language generation

  ???

- Sequence-to-sequence Data Augmentation for Dialogue Language Understanding.  COLING 2018 [code](https://github.com/AtmaHou/Seq2SeqDataAugmentationForLU)

  - [x] data augmentation

    用户输入多样性拓展生成

    ???

- 

---

### 2017



---





### 2015

+ Ground Truth for Grammatical Error Correction Metrics  ACL 2015 [code](https://github.com/cnap/gec-ranking)

  - [x] grammar error detection

  ???

+ Semantically Conditioned LSTM-based Natural Language Generation for Spoken Dialogue Systems, EMNLP 2015 [arxiv](https://arxiv.org/abs/1508.01745)

  - [x] semantically
  - [x] natural language generation

  ???

+ Dialogue focus tracking for zero pronoun resolution, NAACL 2015 [paper](http://aclweb.org/anthology/N/N15/N15-1052.pdf)

  - [x] pronoun resolution

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





