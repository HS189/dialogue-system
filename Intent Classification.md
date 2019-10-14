refer:

<https://docs.microsoft.com/en-us/azure/cognitive-services/LUIS/luis-concept-intent>

<https://docs.microsoft.com/en-us/azure/cognitive-services/luis/luis-concept-best-practices>

### Challenge

+ lack of training data

  A often used approach to overcome this issue is to use the data generation tool [chatito](https://rodrigopivi.github.io/Chatito/) developed by Rodrigo Pimentel. Generating sentences out of predefined word blocks can give you a large dataset quickly. Avoid using data generation tools too much, as your model may overfit on your generated sentence structures. 

  

+ similar intents

  it would be better to unifies the similar intents, then use entity to discriminate it.

  For exmaple, if you want to determine negative and positive intentions, such as "I **want** a car" and "I **don't** want a car", you can create a single intent and mark the two different positive and negative terms as an entity.

  For example, "Book a flight" and "Book a hotel" use the same vocabulary of "book a ". This format is the same so it should be the same intent with the different words of flight and hotel as extracted entities.

  For example, BookFlight and FlightCustomerService might be separate intents in a travel app, but BookInternationalFlight and BookDomesticFlight are too similar. If your system needs to distinguish them, use entities or other logic rather than intents.

+ domain or intent ?

  Use a intent classification ?

  Use a domain-intent classification ? (hierarchical label)

  

+ `none` intent

  This intent is the fallback intent, indicated everything outside your application.

  If you do not add any data for the **None** intent, it will forces an utterances that is outside the domain into one of the domain intents.

  How to construct training data for `none` intent ?





###



### STOA

+ <https://paperswithcode.com/task/intent-classification>



### Datasets

+ <https://github.com/sebischair/NLU-Evaluation-Corpora>



### Tools

+ rasa
+ 



### Paper

+ Subword Semantic Hashing for Intent Classification on Small Datasets
+ Geng R, Li B, Li Y, et al. Few-Shot Text Classification with Induction Network[J]. arXiv preprint arXiv:1902.10482, 2019. It's important? [arxiv](https://arxiv.org/pdf/1902.10482v1.pdf) [code](<https://github.com/wuzhiye7/Induction-Network-on-FewRel>) 









