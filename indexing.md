# 🗂️ indexing 

at a higher level, we have some external documents that we want to load and put inside of a retriever, and the goal of this retriever is to fish out some document from external data store that is relevant to the question as input to the retriever.

to start, `embeddings`are numerical represenations of objects (like text, images, audio) that are represented as vectors and are designed to capture meaningful relationships between them, since it is very easy to compare vectors as opposed to words. we also have two options for vector representation,`sparse vectors` or `dense vectors`.

![image](https://github.com/user-attachments/assets/2b311786-2a4d-4597-b983-58a7fc30079c)


### sparse vectors ### 
in `sparse vectors` a very small amount of values are non-zero (ex. a bag-of-words vector containg 10,000 entries may only contain 10 non-zero entries for a single sentence. If the data is high-dimensional with few active features, sparse vectors may be more efficient. sparse vectors are memory efficient, since the only store non-zero indices and values, making it a huge memory optimization. specialized algorithims exist to compute dot product over overlapping non-zero indices

```
  consider this example: 
    A = {2: 3, 4: 4}
    B = {0: 1, 2: 2, 4: 5}
    abs(A[2] - B[2]) + abs(A[4] - B[4]) = 3
```


### dense vectors ### 
in `dense vectors` are stored in a high dimensional space, values are a majority non-zero. however, each dimension is rich and contians relevant information, determined a neural net and compressing these vectors is complex so they use more memory. dense vectors are thus designed to capture semantics relationships between two vectors, hence when two things are similar their vector representations are close in vector space. 


