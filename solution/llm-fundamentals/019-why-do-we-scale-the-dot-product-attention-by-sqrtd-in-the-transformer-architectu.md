# Why do we scale the dot product attention by √dₖ in the Transformer architecture?

**Topic:** LLM Fundamentals

## Source

- [Math behind √dₖ Scaling Factor in Attention](https://outcomeschool.com/blog/scaling-dot-product-attention)

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
