# What are embeddings?

**Topic:** LLM Fundamentals

## Source

- [Embeddings in Machine Learning](https://www.youtube.com/watch?v=LedXW6xl21s)
  - Transcript notes: the embeddings video defines embeddings as vector representations of text, images, audio, or other objects. Objects with similar meaning or properties are placed close together in vector space, enabling similarity search and recommendation.

## Embeddings

Embeddings are dense numeric vectors that represent objects such as text, images, audio, users, or products.

Key points:
- The vector is learned so that semantically similar objects are close under a distance metric such as cosine similarity.
- Embedding models convert raw inputs into vectors; vector databases index those vectors for fast nearest-neighbor search.
- Good embeddings preserve task-relevant meaning, not every detail of the original object.

## Example

Example: an embedding model should place `refund policy` closer to `return policy` than to `GPU memory allocation`.

## Current Software Engineering Use Case

RAG systems embed document chunks and user queries so the application can retrieve relevant context before asking an LLM to answer.
