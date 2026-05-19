# Your RAG retrieval is too slow with a large knowledge base. How do you speed it up?

**Topic:** Retrieval-Augmented Generation (RAG)

## Operational Playbook

Treat this as a production failure mode: reproduce it, constrain the system, improve the weak component, and add evaluation so it does not regress.

Key points:
- Profile the bottleneck first: queue time, retrieval, model latency, token count, or downstream tools.
- Apply caching, batching, streaming, smaller models, quantization, routing, autoscaling, and backpressure.
- Set SLOs and load-test with realistic concurrency before raising limits.

## Example

For example, if a RAG assistant answers without evidence, return `I do not have enough source context` and log the missing-retrieval case for index improvement.

## Current Software Engineering Use Case

Used in enterprise knowledge assistants where employees ask questions over policies, contracts, tickets, and runbooks with citations.
