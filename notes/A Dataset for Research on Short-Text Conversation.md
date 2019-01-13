#### key notes

+ Labeling data for match and rank

  Training data in match: In the labeled pairs, both positive and negative ones are ranked high by some baseline models, and hence more difﬁcult to tell apart. This supervision will naturally tune the model parameters to ﬁnd the real good responses from the seemingly good ones. Please note that without <u>the labeled negative pairs</u>, we need to generate negative pairs with randomly chosen responses, which in most of the cases are too easy to differentiate by the ranking model and cannot fully tune the model parameters.

  Testing test in match: In testing a retrieval-based system, although we can simply use the original responses associated with the query post as positive and treat all the others as negative, this strategy suffers from the problem of spurious negative examples. In other words, with a reasonably good model, the retrieved responses are often good even if they are not the original ones, which brings significant bias to the evaluation.

  Training data in rank: From the labeled data, we can extract triples (x, y+, y−)
  to ensure that score(x, y+) > score(x, y−). Apparently y+ can be selected from labeled positive response of x, while y− can be sampled either from labeled negative negative or randomly selected ones. Since <u>the manually labeled negative instances</u> are top-ranked candidates according to some individual retrieval model and therefore generally yield slightly better results.

