# What are embedding models, and how do they convert text to vectors?

**Topic:** Retrieval-Augmented Generation (RAG)

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
