### Task-Oriented Dialogue System

![Task-Oriented Dialogue System](https://github.com/bifeng/dialogue-system/raw/master/image/Task-Oriented Dialogue System.png)

Probabilistic methods in spoken–dialogue systems, Steve J. Young, 2000 - [paper](http://rsta.royalsocietypublishing.org/content/358/1769/1389.short)

#### Spoken/Natural Language Understanding (SLU/NLU)

+ Semantic Frame Representation

  requires a domain ontology (本体), contains core content (intent, a set of slots with fillers).

+ Pipelined:<br>Domain Classification -> Intent Classification -> Slot Filling

##### Domain/Intent Classification

As an utterance classification task

[Deep belief nets (DBN) - 2011](http://ieeexplore.ieee.org/abstract/document/5947649/)<br>[Deep convec networks (DCN - 2012)](http://ieeexplore.ieee.org/abstract/document/6289054/)<br>[Extension to kernel-DCN - 2012](http://ieeexplore.ieee.org/abstract/document/6424224/)<br>...

##### Slot Filling

As a sequence tagging task

[Yao+, 2013](http://131.107.65.14/en-us/um/people/gzweig/Pubs/Interspeech2013RNNLU.pdf)<br>[Mesnil+, 2015](http://dl.acm.org/citation.cfm?id=2876380)<br>...

##### Joint Semantic Frame Parsing

[Sequence-based, Hakkani-Tur+, 2016](https://www.microsoft.com/en-us/research/wp-content/uploads/2016/06/IS16_MultiJoint.pdf)<br>[Parallel, Liu & Lane, 2016](https://arxiv.org/abs/1609.01454)<br>...

##### Joint SLU

...

##### Contextual LU

...

##### Structural LU

...



#### Dialogue Management (DM)

##### Dialogue State Tracking (DST)

##### Dialogue Policy Optimization



#### Natural Language Generation (NLG)

