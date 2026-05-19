# What are foundation models, and how have they changed AI engineering?

**Topic:** LLM Fundamentals

## Source

- [AI Engineering Explained: LLM, RAG, MCP, Agent, Fine-Tuning, Quantization](https://www.youtube.com/watch?v=lnfWvX66FUk)
  - Transcript notes: the video frames AI engineering around six practical building blocks: LLMs for language generation, RAG for grounding answers in external knowledge, MCP for standardized tool/data integration, agents for goal-directed tool use, fine-tuning for behavior or domain adaptation, and quantization for cheaper deployment.

## Foundation Models

Foundation models are large models pre-trained on broad datasets and reused across many downstream tasks.

Key points:
- They learn reusable representations during large-scale pre-training.
- They are adapted through prompting, RAG, fine-tuning, or tool use instead of training a task model from scratch.
- They changed AI engineering from model-centric experimentation to product engineering around model capabilities, context, data, evaluation, and safety.

## Example

Example: instead of training separate models for ticket classification, summarization, and reply drafting, start with one capable foundation model and adapt it with prompts, retrieval, and evaluations.

## Current Software Engineering Use Case

A support platform can use one foundation model for summarization, classification, drafting, and tool calling, with task-specific prompts and evaluations around each workflow.
