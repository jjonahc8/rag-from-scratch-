# Indexing 

## Motivation
- At a higher level, we have some external documents that we want to load and put inside of a retriever, and the goal of this retriever is to fish out some document from external data store that is relevant to the question as input to the retriever.

- To start, **embeddings** are numerical represenations of objects (like text, images, audio) that are represented as vectors aand are designed to capture meaningful relationships between them, since it is very easy to compare vectors as opposed to words. We also have two options for vector representation, **sparse vectors** or **dense vectors**.

- Sparse vectors can be stored more efficiently and allow us to perform syntax-based comparisons of two sequences. For example, given two sentences; "Bill ran from the giraffe toward the dolphin", and "Bill ran from the dolphin toward the giraffe" we would get a perfect (or near-perfect) match.

Why? Because despite the meaning of the sentences being different, they are composed of the same syntax (e.g., words). And so, sparse vectors would be closely or even perfectly matched (depending on the construction approach).

Where sparse vectors represent text syntax, we could view dense vectors as numerical representations of semantic meaning. Typically, we are taking words and encoding them into very dense, high-dimensional vectors. The abstract meaning and relationship of words are numerically encoded.

<img width="597" alt="Screenshot 2025-06-05 at 22 18 30" src="https://github.com/user-attachments/assets/f6842cb5-c82a-4a1f-ad76-e9bb12c47f11" />

Imagine we create dense vectors for every word in a book, reduce the dimensionality of those vectors and then visualize them in 3D — we will be able to identify relationships. For example, days of the week may be clustered together:

<img width="579" alt="Screenshot 2025-06-05 at 22 18 48" src="https://github.com/user-attachments/assets/867e9ac8-6f4c-4ec3-976a-9d0505e35189" />
