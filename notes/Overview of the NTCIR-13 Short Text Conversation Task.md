#### key points

+ method

  + retrieval-based

    SG01-C-R1.txt deep sentence match, LTR, v1
    SG01-C-R2.txt deep sentence match, LTR, v2
    SG01-C-R3.txt deep sentence match, LTR, v3

  + generation-based

    SG01-C-G1.txt rerank-base-[vae-predata,seq2seq-2dataset]
    SG01-C-G2.txt rerank-base-[vae-predata]
    SG01-C-G3.txt rerank-base-[seq2seq-2dataset]
    SG01-C-G4.txt origin-seq2seq-2dataset
    SG01-C-G5.txt origin-vae-pre-data

+ evaluation

  Evaluation metrics:

  nG@1 (normalized gain at cutoff 1), P+, and nERR@10 (normalized expected reciprocal rank at cutoff 10)

  Labeling strategy:

  (1) Fluent: the comment is acceptable as a natural language text;
  (2) Coherent: the comment should be logically connected and topically relevant to the original post (i.e. the comment makes sense in the eye of the originator of the post);
  (3) Self-sufficient: the assessor can judge that the comment is appropriate by reading nothing other than the post-comment pair;
  (4) Substantial: the comment provides new information in the eye of the originator of the post;
  If either (1) or (2) is untrue, the retrieved comment should be labeled “L0”; if either (3) or (4) is untrue, the label should be “L1”; otherwise, the label is “L2”.





