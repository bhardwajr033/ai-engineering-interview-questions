# Cloud vs on-device Model Deployment for AI applications.

**Topic:** LLMOps and Production AI

## Source

- [Cloud vs On-Device Model Deployment](https://x.com/outcome_school/status/1965643330076991621)

## LLMOps

LLMOps is the practice of deploying, monitoring, evaluating, and governing LLM applications in production.

Key points:
- It covers prompt/model versioning, traces, cost tracking, latency, quality evaluation, guardrails, incident response, and rollback.
- A gateway centralizes provider access, authentication, rate limits, routing, logging, and fallbacks.
- Production systems need continuous evaluation because model, data, and user behavior change over time.

## Example

Example: route requests through a model gateway that records prompt version, model version, latency, token count, cost, and safety outcomes.

## Current Software Engineering Use Case

An AI platform team uses an LLM gateway and observability stack to control spend, detect regressions, and switch providers during outages.
