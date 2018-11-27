#### key points

- How to extract a proper dependency relation path to represent the sentence?

  Define a relationship path (or simply path) between two nodes of dependency tree as the series of edges, and traverse every two node as the relation path.

  1. ignore the directions of relations. This is because the roles of terms as
     governor and modifier often change in questions and answers. 

  2. ignore relation paths between two words if they belong to the same chunk (which is usually a noun phrase or a verb phrase).
  3. (question and passage) match only the root forms of open class words (or phrases), such as nouns, verbs and adjectives, when pairing corresponding paths.

- Using IBM statistical translation model 1, and treat the matching score of a dependency relation path from a candidate sentence as the probability of translating to it from its corresponding path in the question.

