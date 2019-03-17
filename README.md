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

- The Design and Implementation of XiaoIce, an Empathetic Social Chatbot, 2018.12, [arxiv](https://arxiv.org/pdf/1812.08989.pdf)

  详细介绍了系统架构和关键组件，包括对话管理器、核心聊天、技能和移情计算模块。在系统设计中考虑了智商（IQ）和情商（EQ），将人机社交聊天作为马尔可夫决策过程（MDP）的决策，并优化了小冰的长期用户参与度和预期的每次会话对话（CPS）。我们展示了小冰如何动态识别人类的感受和状态，理解用户意图，并在长时间的对话中响应用户需求。

- From Eliza to XiaoIce: Challenges and Opportunities with Social Chatbots, 2018.01, [arxiv](https://arxiv.org/abs/1801.01957)

- 全双工语音对话以及在智能硬件上的应用，微软小冰全球首席架构师及研发总监周力，2019.01.17

- 微软小冰与情感计算框架，微软（亚洲）互联网工程院副院长李笛，2019.01.10 [ppt and video](https://pan.baidu.com/s/1jTM0J9kqnG_Jl1cfsAUdMA)

- 微软小冰技术交流会，微软（亚洲）互联网工程院，2018.03.28

  全双工语音交互感官（Full-duplex Voice Sense）

- 研发人员

  微软亚洲研究院 [people](https://www.microsoft.com/en-us/research/group/natural-language-computing/?from=http%3A%2F%2Fresearch.microsoft.com%2Fen-us%2Fgroups%2Fnlc%2F)

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



## Conference

+ SIGdial (Special Interest Group on Discourse and Dialogue) 

  https://www.sigdial.org/



## Challenge

+ DSTC (Dialog State/System Tracking Challenge)

  DSTC1

  Domain - Bus Route

  Task - Evaluation Metrics

  DSTC2

  Domain - Restaurant

  Task - User Goal Changes

  DSTC3

  Domain - Tourist Information

  Task - Domain Adaptation

  DSTC4

  Domain - Tourist Information

  Task - Human Conversation

  DSTC5

  Domain - Tourist Information

  Task - Language Adaptation

  DSTC6

  <details><summary>Track</summary>
      End-to-End Goal-Oriented Dialog Learning<br>
      End-to-End Conversation Modeling<br>
      Dialogue Breakdown Detection

  DSTC7

  http://workshop.colips.org/dstc7/call.html

  <details><summary>Track</summary>
      Sentence Selection: goal-oriented multi-turn dialog<br>
      Sentence Generation<br>
      Audio Visual Scene-aware dialog (AVSD)
  </details>


  Workshop (paperlist) - http://workshop.colips.org/dstc7/workshop.html

  Sentence Selection:

  1st place - [paper](http://workshop.colips.org/dstc7/papers/07.pdf) | [slide](http://workshop.colips.org/dstc7/papers/DSTC7-Track1-QianChen.pdf) 

+ SLT 2018 Microsoft Dialogue Challenge: Building End-to-End Task-Completion Dialogue Systems

  https://github.com/xiul-msr/e2e_dialog_challenge

  <details><summary>Task</summary>
      Movie-Ticket Booking<br>
      Restaurant Reservation<br>
      Taxi Ordering<br>
  </details>

+ ConvAI (The Conversation Intelligence Challenge)

  https://github.com/DeepPavlov/convai

  ConvAI2

  Track - Persona-Chat

  Personalizing Dialogue Agents: I have a dog, do you have pets too?, 2018 [arxiv](https://arxiv.org/abs/1801.07243) 

  the winner has been announced: ["Lost in Conversation"](https://github.com/atselousov/transformer_chatbot)! See the presentation slides for all details: [intro](https://github.com/DeepPavlov/convai/blob/master/NeurIPSConvAI2-IntroPres.pptx), [results](https://github.com/DeepPavlov/convai/blob/master/NeurIPSConvAI2ResultsPres.pptx), [top team presentations](https://github.com/DeepPavlov/convai/blob/master/NeurIPSParticipantSlides.pptx), and [future work](https://github.com/DeepPavlov/convai/blob/master/NeurIPSConvAI2FutureWork.pptx).

  	ConvAI1<br>	http://convai.io/2017/<br>	Track - The aim of the competition was to implement a bot capable of conversing with humans based on a given passage of text.<br>	[1st place](https://github.com/sld/convai-bot-1337) 



## Competition

+ TREC


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
  +  Single-round, chatbot
  +  retrieval
  +  Overview of the NTCIR-12 Short Text Conversation Task, [paper](http://research.nii.ac.jp/ntcir/workshop/OnlineProceedings12/pdf/ntcir/OVERVIEW/01-NTCIR12-OV-STC-ShangL.pdf) | [slides](http://research.nii.ac.jp/ntcir/workshop/OnlineProceedings12/pdf/ntcir/OVERVIEW/01-NTCIR12-OV-STC-ShangL_slides.pdf) 

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

+ Unsupervised Learning and Modeling of Knowledge and Intent for Spoken Dialogue Systems, Yun-Nung (Vivian) Chen, Ph.D. dissertation [pdf](https://www.csie.ntu.edu.tw/~yvchen/publication.html#thesis) 

### 2018

+ Deep Chit-Chat: Deep Learning for ChatBots, Wei Wu and Rui Yan, EMNLP [ppt](http://www.ruiyan.me/pubs/tutorial-emnlp18.pdf) | [video](https://vimeo.com/305179403) | [paper](http://ruiyan.me/pubs/IJCAI2018.pdf) 

  微软小冰首席科学家武威

  北京大学助理教授严睿

  :star::star::star::star::star:

+ Neural Approaches to Conversational AI, Jianfeng Gao, [arxiv](https://arxiv.org/abs/1809.08267)

  Neural Approaches to Conversational AI ACL 2018 [ppt](https://www.microsoft.com/en-us/research/uploads/prod/2018/07/neural-approaches-to-conversational-AI.pdf) 

  :star::star::star::star::star:

- Deep Learning for Dialogue Systems, COLING 2018 [site](https://sites.google.com/view/deepdial/) | [paper](http://aclweb.org/anthology/C18-3006) | [slide](https://www.csie.ntu.edu.tw/~yvchen/doc/COLING18_Tutorial.pdf) 

  :star::star::star::star::star:

- A Survey on Dialogue Systems: Recent Advances and New Frontiers, JD [arxiv](https://arxiv.org/abs/1711.01731) 


### 2017

+ Teaching Machines to Converse, Jiwei Li's Thesis 2017 [code](https://github.com/jiweil/Jiwei-Thesis) | [thesis](https://github.com/jiweil/Jiwei-Thesis/blob/master/thesis.pdf)


### Question

+ Neural approaches in spoken language understanding is just for domain or intent detection and slot filling?

## Scholar

+ Maxine Eskenazi [site](http://www.cs.cmu.edu/~max/) 

  Tiancheng Zhao [site](https://www.cs.cmu.edu/~tianchez/) | [github](https://github.com/snakeztc) <u>task-oriented dialog generation</u> :star::star::star::star::star:

   

  

## Paper notes

Neural Network Dialog System Papers [github](https://github.com/snakeztc/NeuralDialogPapers) active :star::star::star::star::star:

deeplearning-papernotes [github](https://github.com/sld/deeplearning-papernotes) active

chatbots [github](https://github.com/minghui/chatbots) - product attention, such as AliMe!!!

chatbots [github](https://github.com/fuzhenxin/Personal-Emotional-Stylized-Dialog) - personalized, emotional, and stylized  attention!!!

chatbots [github](https://github.com/IsaacChanghau/DL-NLP-Readings/blob/master/readme/nlp/dialogue.md) - 2018

chatbots [github](https://github.com/ricsinaruto/Seq2seqChatbots/wiki/Chatbot-and-Related-Research-Paper-Notes-with-Images) - 2017

## Paper

### personality

- Learning Personalized End-to-End Goal-Oriented Dialog, [Liangchen Luo](https://www.luolc.com/), Wenhao Huang, Qi Zeng, Zaiqing Nie, Xu Sun, AAAI-19 [arxiv](https://arxiv.org/abs/1811.04604) 

  https://mp.weixin.qq.com/s/AqzdRoXthrUFUOqSNwgfqQ

- Assigning personality/identity to a chatting machine for coherent conversation generation, Qiao Qian, Minlie Huang, Haizhou Zhao, Jingfang Xu, Xiaoyan Zhu, IJCAI 2018 [arxiv](https://arxiv.org/abs/1706.02861) | [code](https://github.com/qianqiao/AssignPersonality) | [data](http://coai.cs.tsinghua.edu.cn/hml/dataset/) 

  personality, includes name, gender, age, location, weight, constellation, hobby, idol, speciality, employer - extracted from Weibo Dataset with regular expression patterns.

  为了可控性，可以直接用正则表达式解决！

### sentimental


- Emotional Chatting Machine: Emotional Conversation Generation with Internal and External Memory, Hao Zhou, Minlie Huang, Tianyang Zhang, Xiaoyan Zhu, Bing Liu, AAAI 2018 [arxiv](https://arxiv.org/abs/1704.01074) | [data](http://coai.cs.tsinghua.edu.cn/hml/dataset/) | [code](http://coai.cs.tsinghua.edu.cn/publications/)

  - [x] natural language generation


### ellipses 


- Building an Ellipsis-aware Chinese Dependency Treebank for Web Text, Xuancheng Ren, Xu Sun, Ji Wen, Bingzhen Wei, Weidong Zhan, Zhiyuan Zhang, 2018, [arxiv](https://arxiv.org/abs/1801.06613) | [code](https://github.com/lancopku/Chinese-Dependency-Treebank-with-Ellipsis) 

### data augmentation

- Sequence-to-sequence Data Augmentation for Dialogue Language Understanding. Yutai Hou, Yijia Liu, Wanxiang Che, Ting Liu, COLING 2018 [code](https://github.com/AtmaHou/Seq2SeqDataAugmentationForLU)

  - [x] a sequence-to-sequence generation based data augmentation framework

    用户输入多样性拓展生成


### sentence function

+ Generating Informative Responses with Controlled Sentence Function, 柯沛、关健、黄民烈、朱小燕. ACL 2018 [paper](http://aclweb.org/anthology/P18-1139) | [data](http://coai.cs.tsinghua.edu.cn/hml/dataset/) | [code](https://github.com/kepei1106/SentenceFunction) 

### semantically

+ Semantically Conditioned LSTM-based Natural Language Generation for Spoken Dialogue Systems, Tsung-Hsien Wen, Milica Gasic, Nikola Mrksic, Pei-Hao Su, David Vandyke, Steve Young, EMNLP 2015 [arxiv](https://arxiv.org/abs/1508.01745) | [code](https://github.com/hit-computer/SC-LSTM) 



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





