# Explain Self-RAG. How does the model decide when to retrieve?

**Topic:** Retrieval-Augmented Generation (RAG)

## Advanced Retrieval

Advanced retrieval techniques improve recall and reasoning beyond a single query-vector lookup.

Key points:
- Query transformation rewrites, expands, decomposes, or abstracts the query before search.
- HyDE generates a hypothetical answer/document and embeds it to retrieve conceptually relevant chunks.
- Multi-hop retrieval iteratively finds evidence needed to answer questions requiring several facts.

## Example

Example: decompose `Which deployment caused the outage and who approved it?` into searches over incidents, deploy logs, and approval records.

## Current Software Engineering Use Case

Incident-analysis assistants use query decomposition to retrieve logs, deployment notes, and runbooks before producing a root-cause summary.
