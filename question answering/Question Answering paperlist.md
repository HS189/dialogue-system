NLP progress<br>https://github.com/sebastianruder/NLP-progress/blob/master/english/question_answering.md



### Challenge

+ 如何判断材料中没有答案，或者答案在材料中多次出现？
+ 



### Awesome

+ awesome question answering [github](https://github.com/dapurv5/awesome-question-answering) 
+ 

### Methods

#### Combined

#### Knowledge Based :star::star::star::star::star:

#### Generation Based

#### Retrieval Based



### Literature Review

+ Hang Li, Will Question Answering Become Main Theme of IR Research? Keynote Speech at the 12th Asia Information Retrieval Societies Conference (AIRS'16), Tsinghua University, December 2016. ([pdf](http://www.hangli-hl.com/uploads/3/4/4/6/34465961/airs_2016_question_answering.pdf))

+ A Review on Deep Learning Techniques Applied to Answer Selection, COLING 2018 [paper](https://aclweb.org/anthology/C18-1181) 

+ Deep Learning for Answer Sentence Selection, NIPS 2014 [arxiv](https://arxiv.org/abs/1412.1632) | [code](https://github.com/brmson/Sentence-selection) 

  

+ A Survey of Text Question Answering Techniques, 2012 [paper](http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.258.7801&rep=rep1&type=pdf) 

+ Biomedical question answering: A survey, 2010 [paper](http://research.cis.drexel.edu:8080/sofia/pub/CMPB_Paper.pdf)

+ A Survey of Answer Extraction Techniques in Factoid Question Answering, 2006 [paper](https://nlp.stanford.edu/mengqiu/publication/LSII-LitReview.pdf) 

  

### Paper

#### multi-hop question answering

- Commonsense for Generative Multi-Hop Question Answering Tasks, Lisa Bauer, Yicheng Wang, Mohit Bansal, EMNLP 2018 [arxiv](https://export.arxiv.org/abs/1809.06309) | [code](https://github.com/yicheng-w/CommonSenseMultiHopQA) 
  - [x] multi-hop question answering

#### Knowledge Based

- Strong Baselines for Simple Question Answering over Knowledge Graphs with and without Neural Networks, Salman Mohammed, Peng Shi, Jimmy Lin, NAACL HLT 2018, [paper](http://aclweb.org/anthology/N18-2047) | [code](https://github.com/castorini/BuboQA) 
- Question Answering on Knowledge Bases and Text using Universal Schema and Memory Networks, Rajarshi Das, Manzil Zaheer, Siva Reddy, Andrew McCallum, ACL 2017 [arxiv](https://arxiv.org/abs/1704.08384) | [code](https://github.com/rajarshd/TextKBQA) 

#### Relation Based

- An Interpretable Reasoning Network for **Multi-Relation** question answering, Mantong Zhou, Minlie Huang, Xiaoyan Zhu, COLING 2018, [paper](https://www.aclweb.org/anthology/C18-1171) | [arxiv](https://arxiv.org/abs/1801.04726) 
- 

#### learning to rank

- Learning to Rank Short Text Pairs with Convolutional Deep Neural Networks, Aliaksei Severyn，Alessandro Moschitti. SIGIR, 2015 [code](https://github.com/aseveryn/deep-qa) 

  **Question**: match question and answer sentences, how to solve the entities association problem? 

#### Reading Comprehension

[基于CNN的阅读理解式问答模型：DGCNN](https://kexue.fm/archives/5409) 

+ Dataset and Neural Recurrent Sequence Labeling Model for Open-Domain Factoid Question, [arxiv](https://arxiv.org/abs/1607.06275) 

  1、直接将问题用LSTM编码后得到“问题编码”，然后拼接到材料的每一个词向量中；

  2、人工提取了2个共现特征；

  3、将最后的预测转化为了一个序列标注任务，用CRF解决。

+ 



WebQA式问答，材料中不一定有答案，所以我们不用softmax，而是对整个序列都用sigmoid，这样既允许了材料中没有答案，也允许答案在材料中多次出现。



##### Pointer Network

+ 

在SQUAD的评测中，材料是肯定有答案的，并且答案所在的位置也做好了标注，所以SQUAD的模型一般是对整个序列做两次softmax，来预测答案的开始位置和终止位置，我们一般称之为“指针网络”。



#### Text Match

- Improved Representation Learning for Question Answer Matching, ACL 2016 [paper](http://www.aclweb.org/anthology/P/P16/P16-1044.pdf) 

  Challenges: 

  1. the task of supporting passage selection for factoid QA may be largely cast as a textual entailment problem

  2. the linguistic similarities between questions and answers may or may not be
     indicative for our task. 

     This is because, depending on what the question is looking for, a good answer may come in different forms: 

     sometimes a correct answer completes the question precisely with the missing information, and in other scenarios, good answers need to elaborate part of the question to rationalize it, and so on. 

     Additionally, while a good answer must relate to the question, they often do
     not share common lexical units.

  3. ...

#### answer seletion

+ A Review on Deep Learning Techniques Applied to Answer Selection – Tuan Manh Lai, Trung Bui and Sheng Li. COLING 2018 [paper](https://aclanthology.info/papers/C18-1181/c18-1181) 
+ Exploring the Effectiveness of Convolutional Neural Networks for Answer Selection in End-to-End Question Answering, Royal Sequiera, Gaurav Baruah, Zhucheng Tu, Salman Mohammed, Jinfeng Rao, Haotian Zhang, Jimmy Lin, SIGIR 2017 [arxiv](https://arxiv.org/abs/1707.07804) 
+ LSTM-based Deep Learning Models for Non-factoid Answer Selection, Ming Tan, Cicero dos Santos, Bing Xiang, Bowen Zhou, ICLR 2016 [arxiv](https://arxiv.org/abs/1511.04108) 
+ Applying Deep Learning to Answer Selection: A Study and An Open Task, Minwei Feng, Bing Xiang, Michael R. Glass, Lidan Wang, Bowen Zhou, ASRU 2015 [arxiv](https://arxiv.org/abs/1508.01585) 
+ 

#### passage retrieval

- Question Answering Passage Retrieval Using Dependency Relations, SIGIR 2005. [paper](https://www.comp.nus.edu.sg/~kanmy/papers/f66-cui.pdf) | [slides](https://www.comp.nus.edu.sg/~kanmy/papers/deppass_draft_v0.5.htm) :star::star::star:

