# How do you handle cold start latency for serverless AI deployments?

**Topic:** AI Infrastructure and Scalability

## Operational Playbook

Treat this as a production failure mode: reproduce it, constrain the system, improve the weak component, and add evaluation so it does not regress.

Key points:
- Profile the bottleneck first: queue time, retrieval, model latency, token count, or downstream tools.
- Apply caching, batching, streaming, smaller models, quantization, routing, autoscaling, and backpressure.
- Set SLOs and load-test with realistic concurrency before raising limits.

## Example

For example, if a RAG assistant answers without evidence, return `I do not have enough source context` and log the missing-retrieval case for index improvement.

## Current Software Engineering Use Case

Used by software teams building ai infrastructure and scalability features that must balance quality, latency, cost, safety, and maintainability.
