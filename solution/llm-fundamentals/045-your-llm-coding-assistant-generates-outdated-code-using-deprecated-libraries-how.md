# Your LLM coding assistant generates outdated code using deprecated libraries. How do you fix it?

**Topic:** LLM Fundamentals

## Operational Playbook

Treat this as a production failure mode: reproduce it, constrain the system, improve the weak component, and add evaluation so it does not regress.

Key points:
- Attach current documentation through RAG or tool access instead of relying on model memory.
- Version indexes and prompts so stale outputs can be traced and rolled back.
- Continuously evaluate against recent examples from production.

## Example

For example, if a RAG assistant answers without evidence, return `I do not have enough source context` and log the missing-retrieval case for index improvement.

## Current Software Engineering Use Case

Used in developer tools for code generation, review, migration, test writing, and repository-aware assistance.
