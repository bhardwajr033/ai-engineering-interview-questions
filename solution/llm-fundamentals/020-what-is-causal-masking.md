# What is causal masking?

**Topic:** LLM Fundamentals

## Source

- [Causal Masking in Attention](https://outcomeschool.com/blog/causal-masking-in-attention)

## Causal Masking

Causal masking prevents a decoder-only model from attending to future tokens during training and inference.

Key points:
- The mask blocks attention from position i to positions greater than i.
- It preserves the next-token prediction objective by ensuring each token only sees prior context.
- It enables parallel training while maintaining autoregressive behavior.

## Example

Example: while predicting token 5 during training, the model may attend to tokens 1-4 but not token 6 or later.

## Current Software Engineering Use Case

Every chat completion model uses causal masking so it can generate responses one token at a time without leaking the target output during training.
