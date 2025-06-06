# 🗂️ indexing 

at a higher level, we have some external documents that we want to load and put inside of a retriever, and the goal of this retriever is to fish out some document from external data store that is relevant to the question as input to the retriever.

to start, `embeddings`are numerical represenations of objects (like text, images, audio) that are represented as vectors and are designed to capture meaningful relationships between them, since it is very easy to compare vectors as opposed to words. we also have two options for vector representation,`sparse vectors` or `dense vectors`.

![image](https://github.com/user-attachments/assets/2b311786-2a4d-4597-b983-58a7fc30079c)

in sparse vectors a very small amount of values are non-zero (ex. a bag-of-words vector containg 10,000 entries may only contain 10 non-zero entries for a single sentence. 
- sparse vectors are memory efficient, since the only store non-zero indices and values, making it a huge memory optimization.
- specialized algorithims exist to compute dot product over overlapping non-zero indices

` 
  A = {2: 3, 4: 4}
  B = {0: 1, 2: 2, 4: 5}
  A[2] * B[2] + A[4] * B[4] 
` 









