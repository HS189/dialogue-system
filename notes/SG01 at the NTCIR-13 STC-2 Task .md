#### key points

#### retrieval based

+ retrieve

  a dozen of traditional features used in web search engine, such as BM25, MRF for term dependency, Proximity, etc.

+ match

  cosine similarity between TF-IDF vector of query and post
  cosine similarity between TF-IDF vector of query and comment
  cosine similarity between TF-IDF vector of query and post + comment
  negative Word Mover Distance between query and post
  negative Word Mover Distance between query and comment
  negative Word Mover Distance between query and post + comment

  translation based language model score between query and comment

+ ranking

  features: 

  Beside all the features’ scores aforementioned, there are newly generated matching scores at this stage:

  - representation based match with a ranking based objective

    use the element-wise sum of word vectors of a sentence as the sentence’s representation, then pass the post’s representation and the comment’s representation through a simple MLP to calculate a matching score

  - representation based match with a ranking based objective

    use combines Bidirectional LSTM and CNN to get the representation of a sentence, then pass the post’s representation and the comment’s representation through another MLP to calculate another matching score

  - seq2seq models used in our generation-based method to calculate another two kinds of matching scores: one model trained by post-comment pairs, another trained by comment-post pairs.

  ranking:

  LambdaMART


#### generation based

+ generate

  S2SAttn uses the basic encoder-decoder framework and the attention mechanism to model the post-comment pairs

  S2SAttn-addmem introduces dynamic memory to the attention mechanism of S2SAttn model. At each time step during decoding, we tail the decoder’s output to encoder’s
  outputs to acquire an augmented memory for computing attention vectors.

  VAEAttn introduces a random variable z into the seq2seq framework, providing a stronger modeling capability for those pairs in which a variety of comments are found to one post. This randomness also allows the model to generate different valid comments for identical inputs.

  We use Segment-beam-search to further increase the diversity of generated sequences.

+ ranking

  features:

  + seq2seq models used in our generation-based method to calculate another two kinds of matching scores: one model trained by post-comment pairs $score_{s2s-p2c}$, another trained by comment-post pairs $score_{s2s-c2p}$.

  ranking:
  $$
  score = \frac{\lambda * \sum_{k}(score_{s2s-p2c})_k + (1-\lambda) * \sum_{k}(score_{s2s-c2p})_k}{lp(R')}
  $$
  $lp(R')$ is a discount ratio, it is used to alleviate the bias caused by sequence length in machine translation task. 
  $$
  lp(R') = \frac{(c+\|R'\|)^\alpha}{(c+1)^\alpha}
  $$


  $\|R'\|$ is the length of candidate response.



