# How do you evaluate multi-turn conversation quality?

**Topic:** Evaluation and Testing

## Memory

AI memory is the state an application preserves and supplies so the model can behave consistently over time.

Key points:
- Short-term memory is recent conversation or task state in the prompt.
- Long-term memory stores durable facts, preferences, summaries, or embeddings outside the context window.
- Episodic memory records past interactions; semantic memory stores general facts.

## Example

Example: a customer-support assistant stores a compact summary of prior issues and retrieves it when the same customer returns.

## Current Software Engineering Use Case

A customer-support assistant stores account preferences and prior issue summaries so users do not repeat context every session.
