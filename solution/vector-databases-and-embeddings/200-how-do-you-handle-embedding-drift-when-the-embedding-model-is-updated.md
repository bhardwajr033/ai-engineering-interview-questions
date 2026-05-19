# How do you handle embedding drift when the embedding model is updated?

**Topic:** Vector Databases and Embeddings

## Operational Playbook

Treat this as a production failure mode: reproduce it, constrain the system, improve the weak component, and add evaluation so it does not regress.

Key points:
- Attach current documentation through RAG or tool access instead of relying on model memory.
- Version indexes and prompts so stale outputs can be traced and rolled back.
- Continuously evaluate against recent examples from production.
- Compare recent traffic against a stable golden dataset and previous model/index versions.
- Check data, prompt, model, embedding, index, and dependency changes independently.
- Roll back quickly, then add regression tests for the missed failure mode.

## Example

For example, if a RAG assistant answers without evidence, return `I do not have enough source context` and log the missing-retrieval case for index improvement.

## Current Software Engineering Use Case

Used by software teams building vector databases and embeddings features that must balance quality, latency, cost, safety, and maintainability.
