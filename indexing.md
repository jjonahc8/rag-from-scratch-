# indexing 

## motivation
- At a higher level, we have some external documents that we want to load and put inside of a retriever, and the goal of this retriever is to fish out some document from external data store that is relevant to the question as input to the retriever.

to start, **embeddings** are numerical represenations of objects (like text, images, audio) that are represented as vectors aand are designed to capture meaningful relationships between them, since it is very easy to compare vectors as opposed to words. we also have two options for vector representation, **sparse vectors** or **dense vectors**.

a sparse vector is useful when your data is high-dimensional with many zero values, common in areas such as nlp, search, or recommendation systems, with distinct non-zero values. an example being search engines rely heavily on sparse vectors to power queries, when you search a term, the engine matches it against a vast dn of indexed documents using parse vector recommendations, due to efficiency and exact term sort of string matching capable of sparse vectors. 




