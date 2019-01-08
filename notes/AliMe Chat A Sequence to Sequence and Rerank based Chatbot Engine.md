#### key points

+ architecture
  + retrieve - an IR model

    using query with retrieve questions

    query - word segment, stop words remove, synonyms extend

    BM25

  + generative - a generation based model 

    modeling query with candidate answer

    an attentive Seq2Seq model 

  + a re-rank model

    score candidate answers with regarding to query. If the candidate answers has a score higher than a certain **threshold**, it will be taken as the answer; otherwise the answer will be offered by a generation based model.

    an attentive Seq2Seq model to optimize the joint results of IR and generation models.


+ an attentive Seq2Seq model

  ...

  an alignment model that scores how well the input at position $j$ matches to the output at $i - 1$.

  paper:

  Dzmitry Bahdanau, Kyunghyun Cho, and Yoshua Bengio. Neural machine translation by jointly learning to align and translate. In Proceedings of ICLR 2015 .

+ **evaluation**

  Three graded labels: 

  “0” for unsuitable

  “1” means that the answer is only suitable in certain contexts

  “2” indicates that the answer is suitable. 

  To determine whether an answer is suitable or not, we define five evaluation
  rules, namely “right in grammar”, “semantically related”, “well-spoken language”, “context independent” and “not overly generalized”. An answer will be labeled as suitable only if it satisfies all the rules, neutral if it satisfies the first three and breaks
  either of the latter two, and unsuitable otherwise.



