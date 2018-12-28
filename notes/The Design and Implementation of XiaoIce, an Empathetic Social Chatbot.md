### key points

#### General Chat/Domain Chats

##### response candidate retrieval/generation

+ retrieval

  Lucene

  keyword search and semantic search

  + paper:

    Learning distributed representations of data in community question answering for question retrieval. ACM 2016

    Ranking responses oriented to conversational relevance in chat-bots. COLING 2016

  Advantage: the retrieval-based provides high-quality responses for popular topics

+ knowledge graph

  Lucene

  1. topic identification (contextual user query)

  2. query expansion (using knowledge graph (KG) retrieve up to n most related topics, These topics are scored by their relevance using a boosted tree ranker[1] trained on manually labeled training data.)

  3. form a query by combines the query topics and their related topics to retrieve from document (sentences) as response candidates.

  KG - a collection of head-relation-tail triples

  + paper:

    [1] Adapting boosting for information retrieval measures. 2010

  Advantage: It can cover a much broader range of topics, and responses are much longer with more useful content.

+ generation

  the sequence-to-sequence (seq2seq) framework used for conversation response generation

  + paper:

    ...

  Advantage: the generation-based offers robustness and high coverage

##### response candidate ranking

+ a ranking score based on four categories of features:

  Local cohesion features (DSSMs)

  Global coherence features (DSSMs)

  Empathy matching features

  Retrieval matching features (word level, such as BM25 and TFIDF scores, semantic level, such as DSSM scores)

+ paper:

  DSSMs...

  [1] Adapting boosting for information retrieval measures. 2010

#### Dialogue Manager

##### Global State Tracker

##### Dialogue Policy

##### Topic Manager



#### Hierarchical Decision-Making



#### Personality



#### Evaluate

To evaluate the effectiveness of XiaoIce as an AI companion to human users with emotional connections, we use the metric of CPS which indicates on average users’ willingness to share time with XiaoIce via conversation.

Conversation-turns Per Session (CPS) as the success metric for social chatbots. It is the average number of conversation-turns between the chatbot and the user in a conversational session. The larger the CPS is, the better engaged the social chatbot is.





