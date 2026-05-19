# Explain Layer Normalization

**Topic:** LLM Fundamentals

## Source

- [Batch Normalization vs Layer Normalization](https://outcomeschool.com/blog/batch-normalization-vs-layer-normalization)

## Normalization

LayerNorm and RMSNorm stabilize Transformer training by normalizing activations within each token representation.

Key points:
- LayerNorm normalizes using mean and variance across hidden dimensions.
- RMSNorm normalizes by root mean square and usually omits mean subtraction, making it simpler and faster.
- Pre-norm Transformer blocks improve gradient flow in deep models.

## Example

Example: RMSNorm keeps activation scale stable in a deep decoder-only LLM while using less computation than full LayerNorm.

## Current Software Engineering Use Case

Modern LLM architectures often use RMSNorm to reduce compute while maintaining stable training and inference.
