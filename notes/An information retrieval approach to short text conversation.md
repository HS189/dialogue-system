### key phases

+ retrieve based, system architecture, motivation, difficulty

#### key points

- System architecture

  ![architecture](https://github.com/bifeng/dialogue-system/raw/master/image/retrieve_based_system_architecture.png)

  **Stage I (retrieval)**, the system employs three fast basic linear matching models to retrieve a number of candidate post-comment pairs for the given query q, forming a reduced candidate set C.
  **Stage II (matching)**, the system utilizes more matching models to further evaluate all the comments in C, returning a matching feature set for each candidate post-comment pair. The matching models are learned offline with techniques referred to as learning to match.
  **Stage III (ranking)**, the system uses a linear ranking function with the matching models as features to further evaluate all the comments (responses) in C, and assigns a ranking score to each candidate comment. Then, the system ranks the candidate comments based on their scores and selects the comment with the highest score to respond. The linear ranking function is learned off-line with learning to rank techniques.

+ retrieval

+ matching

  Matching Features

  Query-Response Similarity, Query-Response Matching in Latent Space, Deep Semantic Matching Model (Query-Response), **Query-Post Similarity**

  Translation-based Language Model (Query-Post-Response - **The lexical gap problem** there is no word overlap between the candidate responses and the query.)

  Topic-Word Model (Query-Response - **The topic consistency**.)

  Co-occurrence features

  Longest Common String (LCS)

  ...

+ ranking

  linear RankingSVM

+ Failed Issues

  1. entity association

     ![entity association](https://github.com/bifeng/dialogue-system/raw/master/image/entity_association.png)

  2. logic consistency

     ![logic consistency](https://github.com/bifeng/dialogue-system/raw/master/image/logic_consistency.png)

+ evaluation

  Mean Average Precision (MAP) and Precision@1 (P@1).




