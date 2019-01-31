### models

#### retrieval based

##### paper

+ DocChat: An Information Retrieval Approach for Chatbot Engines Using Unstructured Documents, Nan Duan(段楠), ACL 2016 [paper](http://aclweb.org/anthology/P16-1049)

  Intuition: **Current retrieval-based or generation-based methods depend on existing Q-R, for many specific domains, collecting such Q-R pairs is intractable! Retrieve response from documents will not encounter this problem!**

  - [x] retrieval based

+ Learning to Respond with Deep Neural Networks for Retrieval-Based Human-Computer Conversation System, Rui Yan(严 睿), SIGIR 2016 [paper](http://ruiyan.me/) 

  - [x] retrieval based

#### generation based

##### literature review

##### paper

- Response Generation by Context-aware Prototype Editing, Yu Wu, Furu Wei, Shaohan Huang, Yunli Wang, Zhoujun Li, Ming Zhou, AAAI-19 [arxiv](https://arxiv.org/abs/1806.07042) | [code](https://github.com/MarkWuNLP/ResponseEdit)

  - [x] generation based
  - [x] sentence editing

- Neural Response Generation with Dynamic Vocabularies, Yu Wu, Wei Wu, Dejian Yang, Can Xu, Zhoujun Li, Ming Zhou, AAAI18 [arxiv](https://arxiv.org/abs/1711.11191) | [paper and video](链接: https://pan.baidu.com/s/1c298bJi 密码: 6zhj)

  - [x] generation based

    微软小冰首席科学家武威

    北京航空航天大学—微软亚洲研究院联合培养博士生吴俣




- Topic Aware Neural Response Generation, Chen Xing, Wei Wu, Yu Wu, Jie Liu, Yalou Huang, Ming Zhou, Wei-Ying Ma, 2016 [arxiv](https://arxiv.org/abs/1606.08340) 

- A Hierarchical Latent Variable Encoder-Decoder Model for Generating Dialogues. Iulian Vlad Serban, Alessandro Sordoni, Ryan Lowe, Laurent Charlin, Joelle Pineau, Aaron Courville, Yoshua Bengio. 2016. [arxiv](http://arxiv.org/abs/1605.06069) 

  Building End-To-End Dialogue Systems Using Generative Hierarchical Neural Network Models. Iulian V. Serban, Alessandro Sordoni, Yoshua Bengio, Aaron Courville, Joelle Pineau. 2016. AAAI. [arxiv](http://arxiv.org/abs/1507.04808).

  [code](https://github.com/julianser/hed-dlg-truncated)

  - [x] generation based 

    (the Hierarchical Encoder Decoder RNN model (HRED) and the Latent Variable Hierarchical Recurrent Encoder-Decoder RNN model (VHRED))

- 2016 [code](https://github.com/UFAL-DSG/tgen)

  - [x] generation based

    A*-search based generation, seq2seq generation

- A Neural Network Approach to Context-Sensitive Generation of Conversational Responses, Alessandro Sordoni, Michel Galley, Michael Auli, Chris Brockett, Yangfeng Ji, Margaret Mitchell, Jian-Yun Nie, Jianfeng Gao, Bill Dolan, NAACL-HLT, 2015 [arxiv](https://arxiv.org/abs/1506.06714) 



#### combined

##### retrieval/generation

+ Learning Matching Models with Weak Supervision for Response Selection in Retrieval-based Chatbots, Yu Wu, Wei Wu, Zhoujun Li, Ming Zhou, ACL 2018 [arxiv](https://arxiv.org/abs/1805.02333)

  Intuition: **a common practice of the negative sampling strategy is randomly sampled ones as negative examples. This strategy, however, oversimplifies the learning problem, as most of the randomly sampled responses are either far from the semantics of the messages or the contexts, or they are false negatives which pollute the training data as noise. Using a sequence-to-sequence architecture (Seq2Seq) model as a weak annotator to judge the matching degree of unlabeled pairs, then guide the matching model learning more harder examples and makes the model more robust.**

  - [x] retrieval based

  - [x] generation based

    The generation model as the evaluator/annotator of sentence matching.

### Multi-turn Summary

#### key phrases

#### framework

Framework I: embedding -> matching

Framework II: representation -> matching -> aggregation

#### Papers

+ Sequential Matching Network: A New Architecture for Multi-turn Response Selection in Retrieval-based Chatbots, Yu Wu, Wei Wu, Chen Xing, Ming Zhou, Zhoujun Li, ACL. 2017 [arxiv](https://arxiv.org/abs/1612.01627) | [code](https://github.com/MarkWuNLP/MultiTurnResponseSelection) 
  + [x] retrieval based
+ The Ubuntu Dialogue Corpus: A Large Dataset for Research in Unstructured Multi-Turn Dialogue Systems, Ryan Lowe, Nissan Pow, Iulian Serban, Joelle Pineau, SIGDIAL 2015 [arxiv](https://arxiv.org/abs/1506.08909) | [source code](https://github.com/npow/ubottu) | [code](https://github.com/dennybritz/chatbot-retrieval) | [new code](https://github.com/Irvinglove/chatbot-retrieval)
  - [x] datasets
  - [x] retrieval based

### Single-turn Summary

#### key phrases

#### framework

Framework I: matching with sentence embeddings

Framework II: matching with question-response interaction

Extension: matching with external knowledge

#### Papers

+ Neural Responding Machine for Short-Text Conversation, Lifeng Shang, Zhengdong Lu, Hang Li, ACL 2015, [arxiv](https://arxiv.org/abs/1503.02364) | [paper](http://anthology.aclweb.org/P/P15/P15-1152.pdf)

  - [x] generation based

    first important paper using generation based method in conversation

+ An information retrieval approach to short text conversation, Zongcheng Ji, Zhengdong Lu, Hang Li, CS 2014 [arxiv](https://arxiv.org/abs/1408.6988) | [datasets](http://data.noahlab.com.hk/conversation/) - **abstract level version**

  - [x] retrieval based

    first important paper using retrieval based method in conversation

+ A Dataset for Research on Short-Text Conversation, Hao Wang, Zhengdong Lu, Hang Li and Enhong Chen, EMNLP 2013 [paper](http://www.hangli-hl.com/recent-publications.html) - **specific level version**

  - [x] datasets

    sina微博上10个活跃的NLP大牛及其follower，topic都主要集中在Research、General Arts and Science、IT Technology、Life等方面。

  - [x] retrieval based

    first important paper using retrieval based method in conversation







