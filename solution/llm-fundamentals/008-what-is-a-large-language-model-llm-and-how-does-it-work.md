# What is a Large Language Model (LLM), and how does it work?

**Topic:** LLM Fundamentals

## Source

- [AI Engineering Explained: LLM, RAG, MCP, Agent, Fine-Tuning, Quantization](https://www.youtube.com/watch?v=lnfWvX66FUk)
  - Transcript notes: the video frames AI engineering around six practical building blocks: LLMs for language generation, RAG for grounding answers in external knowledge, MCP for standardized tool/data integration, agents for goal-directed tool use, fine-tuning for behavior or domain adaptation, and quantization for cheaper deployment.

## Large Language Models

An LLM is a neural language model, usually Transformer-based, trained to predict or generate text token by token.

Key points:
- Text is tokenized into ids, converted to embeddings, processed by Transformer layers, and decoded into a probability distribution over the next token.
- Generation samples or selects the next token repeatedly until a stop condition is reached.
- LLMs do not retrieve truth by default; they generate likely continuations from learned patterns and supplied context.

## Example

Example: for the prompt `Summarize this incident report`, the model tokenizes the text, attends over the context, then emits summary tokens until it reaches a stop condition.

## Current Software Engineering Use Case

LLMs power coding assistants, document Q&A, customer-support chatbots, data extraction, meeting summaries, and workflow automation.
