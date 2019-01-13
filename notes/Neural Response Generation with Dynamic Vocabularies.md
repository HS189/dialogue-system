#### key notes

+ intuition

  Only a small part of words are useful in the decoding.

  + Function words should be included.
    Function words guarantee grammatical correctness and fluency of responses.
    的，了，我，你….
  + Words that are relevant to the context should be included.
    Content words, on the other hand, express semantics of responses.
  + How to select content words?
    Alignment model does not work for dialogue.
    We need to train a model that capable of allocating a dynamic vocabulary for each input.

+ ideas

  proposal of a dynamic vocabulary sequence-to-sequence model and derivation of a learning approach that can jointly optimize word selection and response generation.

  + Save online decoding time
    It is a time consuming operation to convert a hidden vector into a vocabulary distribution.
    Matrix multiplication is sensitive to the matrix dimension.
  + Filter irrelevant words
    Only a small part of words can be used in the decoding.
    Filter out irrelevant words.

+ vocabulary construction

  Construct a dynamic vocabulary for each input. 

  + static word (include function words)

  + dynamic word (include content words)

    Using the word prediction model, the loss is formulated as:
    $$
    P(w_{pos}=1|X) + p(w_{neg}=0|X)
    $$
    where ${w_{neg}}$ are sampled by **frequency**, and ${w_{pos}}$ are words in the ground-truth response.

    (This negative sampling strategy will often sample high frequency word as negative samples to reduce boring response!)



