# What is a vector database, and how does it differ from a traditional database?

**Topic:** Vector Databases and Embeddings

## Vector Databases

A vector database stores embeddings and retrieves nearest neighbors efficiently using similarity metrics and indexes.

Key points:
- Cosine similarity compares direction, dot product combines direction and magnitude, and Euclidean distance measures geometric distance.
- Approximate nearest-neighbor indexes such as HNSW trade tiny recall loss for much faster search.
- Metadata filtering, tenant isolation, replication, and reindexing are production concerns beyond raw similarity search.

## Example

Example: store embeddings for every documentation chunk and retrieve nearest neighbors to answer semantic queries like `how do I rotate credentials?`.

## Current Software Engineering Use Case

Vector databases back RAG, semantic search, recommendation, duplicate detection, personalization, and multimodal retrieval.
