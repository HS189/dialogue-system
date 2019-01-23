#### key notes

+ Labeling data for Training and Testing

  Training: In the labeled pairs, both positive and negative ones are ranked high by some baseline models, and hence more difﬁcult to tell apart. This supervision will naturally **fine-tuning** the model parameters to ﬁnd the real good responses from the seemingly good ones. Please note that without <u>the labeled negative pairs</u>, we need to generate negative pairs with randomly chosen responses, which in most of the cases are too easy to differentiate by the ranking model and cannot fully tune the model parameters.

  Testing: In testing a retrieval-based system, although we can simply use the original responses associated with the query post as positive and treat all the others as negative, this strategy suffers from the problem of spurious negative examples. In other words, with a reasonably good model, the retrieved responses are often good even if they are not the original ones, which brings significant bias to the evaluation.

+ Techniques

  The training and testing are both performed on the 422 labeled posts, with about 12,000 labeled (post, response) pairs. We use a 5-fold cross validation with a fixed penalty parameter for slack variable.



