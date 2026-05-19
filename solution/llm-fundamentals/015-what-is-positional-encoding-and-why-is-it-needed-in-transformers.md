# What is positional encoding, and why is it needed in Transformers?

**Topic:** LLM Fundamentals

## Source

- [Positional Embeddings in LLMs](https://outcomeschool.substack.com/p/positional-embeddings-in-llms)

## Position Information

Position information tells a Transformer where each token appears, because self-attention alone is order-agnostic.

Key points:
- Absolute or learned positional embeddings add a position vector to each token embedding.
- RoPE rotates query and key vectors by position-dependent angles, encoding relative position directly inside attention scores.
- RoPE tends to extrapolate better than simple learned position embeddings and is common in modern decoder-only LLMs.

## Example

Example: `dog bites man` and `man bites dog` contain the same words, but positional encoding lets the model distinguish the two meanings.

## Current Software Engineering Use Case

Long-context chat models, code assistants, and RAG systems rely on strong positional encoding so the model can distinguish instruction order, document order, and nearby evidence.
