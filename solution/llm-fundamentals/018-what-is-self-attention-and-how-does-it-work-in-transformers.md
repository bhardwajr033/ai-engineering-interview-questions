# What is self-attention, and how does it work in Transformers?

**Topic:** LLM Fundamentals

## Source

- [Math behind Attention - Q, K, and V](https://outcomeschool.com/blog/math-behind-attention-qkv)

## Self-Attention

Self-attention lets each token build a context-aware representation by attending to other tokens in the same sequence.

Key points:
- Attention scores are computed from query-key dot products, normalized with softmax, and used to weight value vectors.
- Causal self-attention masks future tokens so generation cannot look ahead.
- Multi-head attention runs several attention projections in parallel so different heads can capture different relationships.

## Example

Example: in a support ticket, self-attention can connect `it` to the affected product mentioned several sentences earlier.

## Current Software Engineering Use Case

Self-attention lets an LLM connect a pronoun to its entity, a code variable to its declaration, or a user question to relevant retrieved evidence.
