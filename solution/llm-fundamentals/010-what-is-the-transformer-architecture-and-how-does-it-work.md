# What is the Transformer architecture and how does it work?

**Topic:** LLM Fundamentals

## Source

- [Decoding Transformer Architecture](https://outcomeschool.com/blog/decoding-transformer-architecture)

## Transformer Architecture

A Transformer is a neural architecture that uses attention to let each token condition on other relevant tokens in the sequence.

Key points:
- Core blocks include token embeddings, positional information, self-attention, feed-forward networks, normalization, and residual connections.
- Decoder-only Transformers use causal masking for next-token generation; encoder-only models build bidirectional representations; encoder-decoder models map an input sequence to an output sequence.
- Attention makes Transformers highly parallel during training and effective at modeling long-range dependencies.

## Example

Example: in `The service failed because it exhausted memory`, attention helps the token `it` connect back to `service` while later layers form a useful representation for generation.

## Current Software Engineering Use Case

Modern LLM APIs, embedding models, translation systems, code models, and vision-language models are all built on Transformer variants.
