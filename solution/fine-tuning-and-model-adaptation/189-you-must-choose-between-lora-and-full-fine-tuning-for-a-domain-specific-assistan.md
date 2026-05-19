# You must choose between LoRA and full fine-tuning for a domain-specific assistant. How do you decide?

**Topic:** Fine-Tuning and Model Adaptation

## Source

- [LoRA - Low-Rank Adaptation of LLMs](https://outcomeschool.com/blog/lora-low-rank-adaptation-of-llms)

## Operational Playbook

Treat this as a production failure mode: reproduce it, constrain the system, improve the weak component, and add evaluation so it does not regress.

Key points:
- Improve domain data coverage through glossary expansion, domain-specific embeddings, or fine-tuning.
- Add exact keyword and metadata retrieval so rare terms are not lost in semantic search.
- Evaluate on realistic domain queries, abbreviations, synonyms, and edge cases.

## Example

For example, if a RAG assistant answers without evidence, return `I do not have enough source context` and log the missing-retrieval case for index improvement.

## Current Software Engineering Use Case

Used by software teams building fine-tuning and model adaptation features that must balance quality, latency, cost, safety, and maintainability.
