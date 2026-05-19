# You deployed a new embedding model, and search quality crashed overnight. How do you handle embedding drift?

**Topic:** Vector Databases and Embeddings

## Operational Playbook

Treat this as a production failure mode: reproduce it, constrain the system, improve the weak component, and add evaluation so it does not regress.

Key points:
- Compare recent traffic against a stable golden dataset and previous model/index versions.
- Check data, prompt, model, embedding, index, and dependency changes independently.
- Roll back quickly, then add regression tests for the missed failure mode.

## Example

For example, if a RAG assistant answers without evidence, return `I do not have enough source context` and log the missing-retrieval case for index improvement.

## Current Software Engineering Use Case

Used by software teams building vector databases and embeddings features that must balance quality, latency, cost, safety, and maintainability.
