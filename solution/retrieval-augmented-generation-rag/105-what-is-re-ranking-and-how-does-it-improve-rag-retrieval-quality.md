# What is re-ranking, and how does it improve RAG retrieval quality?

**Topic:** Retrieval-Augmented Generation (RAG)

## Re-Ranking

Re-ranking uses a stronger model to reorder retrieved candidates by relevance to the query.

Key points:
- A vector database retrieves a broad top-k cheaply.
- A cross-encoder or LLM then scores query-document pairs more precisely.
- Re-ranking improves precision but adds latency and cost.

## Example

Example: retrieve 50 candidate chunks cheaply, then use a cross-encoder to select the top 5 that actually answer the question.

## Current Software Engineering Use Case

A RAG system may retrieve 50 chunks, rerank them to the best 5, and pass only those to the generator.
