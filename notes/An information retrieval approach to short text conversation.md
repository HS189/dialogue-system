### key phases

+ retrieve based, system architecture, motivation, difficulty

#### key points

- Labeling strategy

  We employ a pooling strategy widely used in information retrieval for getting the instances to label (Voorhees, 2002). More specifically, for a given query, we use each of three basic retrieval models to select top 10 comments, and merge them to form a much reduced candidate set with size $\le​$ 30. Then we assign the comments in the reduced candidate set into “suitable” and “unsuitable” categories.

  Finally, we manually label 422 queries and their associated comments, about 30 comments for each post. Note that (1) the labeling is only on a small subset of the 38,016 posts, and (2) for each selected (query) post, the labeled comments are not originally given to it.

  paper:

  Ellen M Voorhees. 2002. The philosophy of information retrieval evaluation. In Evaluation of cross-language information retrieval systems, pages 355-370, Springer.

- Labeling data for Training and Testing

  Training: We have confirmed that the use of labeled negative instances, instead of randomly selected instances, can yield slightly better results. This is because the negative instances are collected from the top ranked candidates with several simple retrieval models, and thus they are more indicative of the difference between positive and negative instances.

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

+ Techniques

  All the results reported below are based on 5-fold cross-validation on the 422 queries. We also perform a significance test using a paired t-test with a significant level of 0.05.

+ evaluation

  Mean Average Precision (MAP) and Precision@1 (P@1).

- Failed Issues

  1. entity association

     ![entity association](https://github.com/bifeng/dialogue-system/raw/master/image/entity_association.png)

  2. logic consistency

     ![logic consistency](https://github.com/bifeng/dialogue-system/raw/master/image/logic_consistency.png)

- 

#### question

- how to select a proper query sets to query for the calculate of query-post match features? 

  old retrieval methods - the top-10 not include the original post

  current retrieval methods - the top-1 is the original post

  how to improve the precision on the top of it?

  -- retrieval bad case - long tail problem?

  -- retrieval system how to handle it?

- how to training the rank model and avoid over-fitting?


