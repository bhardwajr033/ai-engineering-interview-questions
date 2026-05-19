# What is the context window in LLMs, and why does it matter?

**Topic:** LLM Fundamentals

## Source

- [Context Window in LLMs](https://www.linkedin.com/posts/amit-shekhar-iitbhu_the-context-window-is-the-llms-working-memory-activity-7437754426175672320-MH9c)

## Context Window

The context window is the maximum number of tokens a model can consider in a single request.

Key points:
- It includes system prompts, conversation history, retrieved documents, tool outputs, and the generated response budget.
- Longer context helps with large documents but increases latency, cost, and attention memory.
- Applications usually combine retrieval, summarization, compression, and windowing instead of sending everything.

## Example

Example: a 128K-token model can ingest a long policy packet, but a production RAG system should still retrieve only the clauses relevant to the user's question.

## Current Software Engineering Use Case

A legal-document assistant uses chunking and retrieval to fit only the relevant contract clauses into the model context.
