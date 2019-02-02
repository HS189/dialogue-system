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

