# Your text-only RAG system now needs to handle images and tables. How do you extend it?

**Topic:** Retrieval-Augmented Generation (RAG)

## Operational Playbook

Treat this as a production failure mode: reproduce it, constrain the system, improve the weak component, and add evaluation so it does not regress.

Key points:
- Reproduce the failure with representative examples and traces.
- Identify whether the root cause is data, retrieval, prompting, model behavior, tool use, or infrastructure.
- Apply the smallest reliable fix, then add regression tests and monitoring so the issue is caught earlier next time.

## Example

For example, if a RAG assistant answers without evidence, return `I do not have enough source context` and log the missing-retrieval case for index improvement.

## Current Software Engineering Use Case

Used in enterprise knowledge assistants where employees ask questions over policies, contracts, tickets, and runbooks with citations.
