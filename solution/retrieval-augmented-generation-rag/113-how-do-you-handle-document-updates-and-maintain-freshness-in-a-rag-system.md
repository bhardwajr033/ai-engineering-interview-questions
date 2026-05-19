# How do you handle document updates and maintain freshness in a RAG system?

**Topic:** Retrieval-Augmented Generation (RAG)

## Operational Playbook

Treat this as a production failure mode: reproduce it, constrain the system, improve the weak component, and add evaluation so it does not regress.

Key points:
- Attach current documentation through RAG or tool access instead of relying on model memory.
- Version indexes and prompts so stale outputs can be traced and rolled back.
- Continuously evaluate against recent examples from production.

## Example

For example, if a RAG assistant answers without evidence, return `I do not have enough source context` and log the missing-retrieval case for index improvement.

## Current Software Engineering Use Case

Used in enterprise knowledge assistants where employees ask questions over policies, contracts, tickets, and runbooks with citations.
