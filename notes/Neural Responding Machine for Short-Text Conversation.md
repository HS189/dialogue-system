#### key points

+ The SMT based method

  The statistical machine translation (SMT) based method:

  It treats the response generation as a translation problem, in which the model is trained on a parallel corpus of post-response pairs. But the responses are not semantically equivalent to the posts as in translation, and due to the unnecessary alignment between the "source" post and the "target" response, this method often yield responses with grammatical errors and in rigid forms.

+ the general encoder-decoder framework

  **What's the difference between this model and the SMT based method?**

+ evaluation

  Three levels are assigned to a response with scores from 0 to 2:

  • Suitable (+2): the response is evidently an appropriate and natural response to the post;
  • Neutral (+1): the response can be a suitable response in a specific scenario;
  • Unsuitable (0): it is hard or impossible to find a scenario where response is suitable.
  To make the annotation task operable, the suitability of generated responses is judged from the following five criteria:
  (a) Grammar and Fluency: Responses should be natural language and free of any fluency or grammatical errors;
  (b) Logic Consistency: Responses should be logically consistent with the test post;
  (c) Semantic Relevance: Responses should be semantically relevant to the test post;
  (d) Scenario Dependence: Responses can depend on a specific scenario but should not contradict the first three criteria;
  (e) Generality: Responses can be general but should not contradict the first three criteria;
  If any of the first three criteria (a), (b), and (c) is contradicted, the generated response should be labeled as “Unsuitable”. The responses that are general or suitable to post in a specific scenario should be labeled as “Neutral”.

