# What is hybrid search, and why is it better than pure vector search?

**Topic:** Retrieval-Augmented Generation (RAG)

## Hybrid Search

Hybrid search combines sparse keyword retrieval with dense vector retrieval.

Key points:
- Sparse retrieval is strong for exact terms, ids, names, and rare keywords.
- Dense retrieval is strong for semantic matches and paraphrases.
- Fusion methods such as reciprocal rank fusion combine both result sets robustly.

## Example

Example: query `ERR_CONN_RESET invoice API` benefits from keyword matching for the error code and vector search for semantically related troubleshooting docs.

## Current Software Engineering Use Case

Customer-support search often uses hybrid retrieval so product codes and error messages are matched exactly while natural-language descriptions still work.
