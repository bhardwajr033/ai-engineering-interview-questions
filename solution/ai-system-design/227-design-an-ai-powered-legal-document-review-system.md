# Design an AI-powered legal document review system.

**Topic:** AI System Design

## System Design

A strong answer for `Design an AI-powered legal document review system` should decompose the product into data, model, orchestration, safety, and operations layers.

Key points:
- Clarify requirements: users, latency target, quality bar, compliance needs, traffic, data sources, and human escalation rules.
- Use an API layer that handles authentication, rate limits, request validation, tracing, and model/provider routing.
- Use layout-aware parsing, chunking, embeddings, metadata filters, reranking, citations, and access-control-aware retrieval.
- Separate ingestion/retrieval, orchestration, model calls, post-processing, evaluation, and storage so each part can evolve independently.
- Add offline evals, online monitoring, audit logs, cost controls, and fallback behavior before launch.
- Design for failure: provider outage, bad retrieval, unsafe output, stale data, and overloaded queues.

## Example

Example architecture: client -> API gateway -> orchestrator -> retrieval/tools -> model gateway -> validators -> response store/analytics for Design an AI-powered legal document review system.

## Current Software Engineering Use Case

Used in enterprise knowledge assistants where employees ask questions over policies, contracts, tickets, and runbooks with citations.
