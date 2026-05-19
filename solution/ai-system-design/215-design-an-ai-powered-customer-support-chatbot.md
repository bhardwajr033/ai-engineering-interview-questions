# Design an AI-powered customer support chatbot.

**Topic:** AI System Design

## System Design

A strong answer for `Design an AI-powered customer support chatbot` should decompose the product into data, model, orchestration, safety, and operations layers.

Key points:
- Clarify requirements: users, latency target, quality bar, compliance needs, traffic, data sources, and human escalation rules.
- Use an API layer that handles authentication, rate limits, request validation, tracing, and model/provider routing.
- Separate ingestion/retrieval, orchestration, model calls, post-processing, evaluation, and storage so each part can evolve independently.
- Add offline evals, online monitoring, audit logs, cost controls, and fallback behavior before launch.
- Design for failure: provider outage, bad retrieval, unsafe output, stale data, and overloaded queues.

## Example

Example architecture: client -> API gateway -> orchestrator -> retrieval/tools -> model gateway -> validators -> response store/analytics for Design an AI-powered customer support chatbot.

## Current Software Engineering Use Case

Used in support automation to answer common questions, triage tickets, retrieve account context, and escalate risky cases to humans.
