## key phrases

- architecture, difficulty

## response generation

### neural response generation

#### Challenges

##### The fluency problem

##### The "UNK" problem

##### Boring responses/diversity

Easy to generate responses like “I do not know” "me too" “why”, “haha” etc. (Because these response take up a big proportion in training datasets)
Especially bad on long queries

Methods:

objective-based diversity

Jiwei Li, Michel Galley, Chris Brockett, Jianfeng Gao, and Bill Dolan. A diversity-promoting objective function for neural conversation models. In NAACL’16, pages 110–119, 2016.

ranking-based diversity

dialogue act-based diversity

Tiancheng Zhao, Ran Zhao, and Maxine Eskenazi. Learning discourse-level diversity for neural dialog models using conditional variational autoencoders. In ACL’17, pages 654–664, 2017.



处理对话系统的无聊回复，用反向概率p(source|target)做reranking现在应该已经是标配。再比如Rico Sennrich的成名作之一将Monolingual data 跟seq2seq 模型结合。其实这连个思想在phrase-base MT 里面早就被广发的使用。Neural之前的MT，需要对一个大的N-best list用MERT做 reranking， 反向概率 p(source|target) 以及语言模型概率 p(target)是reranking中feature的标配。

refer: [初入NLP领域的一些小建议](<https://zhuanlan.zhihu.com/p/59184256>) 



#### Methods

##### Latent Variable

##### Topic Aware

##### Rerank

##### CVAE 

conditional variational autoencoders

##### Reinforcement

##### Content Introducing

to generate a sentence with constraint words

###### hard constraint

controllable --> backward and forward generation

two-step --> keyword generation, hard constraint in generation

###### soft constraint

implicit content introducing to generation

Lili Yao, Yaoyuan Zhang, Yansong Feng, Dongyan Zhao, and Rui Yan. Towards implicit content introducing for generative short-text conversation systems. In EMNLP’17, pages 2190–2199, 2017.

#### Question

+ Current methods only concern the sentence fluency, and missing the logic consistency of question and response, how to measure or modeling the cross-sentence level or discourse level or session level fluency? 
+ 

