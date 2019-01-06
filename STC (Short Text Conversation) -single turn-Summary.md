#### keyphases

+ architecture, motivation, difficulty

#### key points

+ single turn conversation

  A Dataset for Research on Short-Text Conversation. EMNLP 2013 [paper](http://www.hangli-hl.com/recent-publications.html)

+ retrieve based

  ![architecture](https://github.com/bifeng/dialogue-system/raw/master/image/retrieve_based_system_architecture.png)

  **Stage I (retrieval)**, the system employs three fast basic linear matching models to retrieve a number of candidate post-comment pairs for the given query q, forming a reduced candidate set C.
  **Stage II (matching)**, the system utilizes more matching models to further evaluate all the comments in C, returning a matching feature set for each candidate post-comment pair. The matching models are learned offline with techniques referred to as learning to match.
  **Stage III (ranking)**, the system uses a linear ranking function with the matching models as features to further evaluate all the comments (responses) in C, and assigns a ranking score to each candidate comment. Then, the system ranks the candidate comments based on their scores and selects the
  comment with the highest score to respond. The linear ranking function is learned offline with learning to rank techniques.

  Matching Features: Query-Response Similarity, Query-Response Matching in Latent Space, Deep Semantic Matching Model (Query-Response), **Query-Post Similarity**, Translation-based Language Model (Query-Post-Response - **The lexical gap problem** between the query and the candidate post-comment pairs.), Topic-Word Model, ...

  An information retrieval approach to short text conversation, CS 2014

+ generative based

  Neural Responding Machine for Short-Text Conversation, ACL 2015 [paper](https://www.aclweb.org/anthology/P15-1152)