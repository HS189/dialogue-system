### Task-Oriented Dialogue System

![Task-Oriented Dialogue System](https://github.com/bifeng/dialogue-system/raw/master/image/Task-Oriented Dialogue System.png)

Probabilistic methods in spoken–dialogue systems, Steve J. Young, 2000 [paper](https://royalsocietypublishing.org/doi/abs/10.1098/rsta.2000.0593) 



#### Spoken/Natural Language Understanding (SLU/NLU)

+ Semantic Frame Representation

  requires a domain ontology (本体), contains core content (intent, a set of slots with fillers).

+ Pipelined:<br>Domain Classification -> Intent Classification -> Slot Filling

##### Domain Ontology

Learning key domain concepts from goal-oriented human-human conversations

Transfer dialogue acts across domains

Language extension

###### paper

...

##### Domain/Intent Classification

(Domain Identification/User Intent Detection)

As an utterance classification task

###### paper

[Deep belief nets (DBN) - 2011](http://ieeexplore.ieee.org/abstract/document/5947649/)<br>[Deep convec networks (DCN - 2012)](http://ieeexplore.ieee.org/abstract/document/6289054/)<br>[Extension to kernel-DCN - 2012](http://ieeexplore.ieee.org/abstract/document/6424224/)<br>...



##### Slot Filling

As a sequence tagging task

###### paper

[Yao+, 2013](http://131.107.65.14/en-us/um/people/gzweig/Pubs/Interspeech2013RNNLU.pdf)<br>[Mesnil+, 2015](http://dl.acm.org/citation.cfm?id=2876380)<br>...

##### Joint Semantic Frame Parsing

Sequence-based: Slot filling and intent prediction in the same output sequence.

Parallel-based: Intent prediction and slot filling are performed in two branches.

###### paper

[Sequence-based, Hakkani-Tur+, 2016](https://www.microsoft.com/en-us/research/wp-content/uploads/2016/06/IS16_MultiJoint.pdf)<br>[Parallel, Liu & Lane, 2016](https://arxiv.org/abs/1609.01454)<br>...

##### Contextual LU

###### paper

...

##### Structural LU

###### paper

...



#### Dialogue Management (DM)

##### Task Lineages 

Task lineages 

Language extension

###### paper



##### Dialogue State Tracking (DST)

Dialogue state: a representation of the system's belief of the user's goal(s) at any time during the dialogue.

Inputs -> current user utterance, preceding system response, results from previous turns

for -> looking up knowledge or making API call(s), generating the next system action/response

Maintain a probabilistic distribution instead of a 1-best prediction for better robustness to SLU errors or ambiguous input.

###### paper



##### Dialogue Policy Optimization

Dialogue management in a RL framework

Goal: select the best action that maximizes the future reward

reward for RL $\simeq$ evaluation for system



###### paper





#### Natural Language Generation (NLG)

Mapping dialogue acts into natural language

Template-based: Define a set of rules to map frames to natural language

Plan-based: Divide the problem into pipeline (sentence plan generator -> sentence plan reranker -> surface realizer)

Class-based: class-based language modeling

RNN-based: rnn-based language modeling

Challenge:<br>handling semantic repetition

Solution:<br>post-processing rules<br>gating mechanism<br>attention

###### paper



##### Contextual NLG



###### paper



##### Structural NLG



###### paper



##### Hierarchical NLG



###### paper



#### End-to-End Neural Dialogue Systems





##### Hierarchical Seq2Seq



###### paper





#### System Evaluation

##### Dialogue model evaluation

Crowd sourcing: <br>User simulator: rule-based user simulator, model-based user simulator



##### Response generator evaluation

Word overlap metrics: <br>Embedding based metrics: 



###### paper



