# What is prompt injection, and what are the different types (direct, indirect)?

**Topic:** AI Safety, Ethics, and Responsible AI

## Prompt Engineering

Prompt engineering designs the instructions, context, examples, and output constraints supplied to an LLM.

Key points:
- Zero-shot prompting gives only the task; one-shot and few-shot prompting add examples.
- Structured prompts specify role, goal, constraints, input data, output schema, and failure behavior.
- Production prompt engineering includes versioning, evaluation, injection defenses, and cost/latency control.

## Example

Example: zero-shot: `Classify sentiment: ...`; one-shot: add one labeled example; few-shot: add several representative examples before the new input.

## Current Software Engineering Use Case

A data-extraction service uses prompt templates plus JSON schema validation and retries to produce reliable structured outputs from messy documents.
