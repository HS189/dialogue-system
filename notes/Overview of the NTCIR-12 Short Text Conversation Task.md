#### key points

+ methods

  retrieval-based

  + chinese

    BUPTTeam-C-R1: [post+cmnt]
    BUPTTeam-C-R2: [post+cmnt+random walk based similary]
    BUPTTeam-C-R3: [post+cmnt+random walk based similary+rank based R1]
    BUPTTeam-C-R4: [post+cmnt+pagerank based similary+time rule]
    BUPTTeam-C-R5: [post+cmnt+pagerank based similary+time rule+rank with R1]

  + japanese

    OKSAT-J-R1: post(full+partial)+cmnt(phrase+word), short sentence, word filter, merge queries
    OKSAT-J-R2: post(full+partial)+cmnt(phrase+word), short sentence, merge multiple queries
    OKSAT-J-R3: difference between mecab and expand mecab, length merge queries.
    OKSAT-J-R4: difference between mecab and expand mecab queries.
    OKSAT-J-R5: This run’s cmnt is all short cmnt of agreement

+ evaluation

  evaluation metrics:

  nG@1

  nERR@10

  P+

  Labeling strategy:

  (1) Coherent: logically connected to the new post;
  (2) Topically relevant: the topic matches that of the new post;
  (3) Context-independent: “good or not” does not depend on situations;
  (4) Non-repetitive: does not just repeat what the new post says;

  If either (1) or (2) is untrue, the retrieved comment should be labeled
  “L0”; if either (3) or (4) is untrue, the label should be “L1”;
  otherwise, the label is “L2”.


