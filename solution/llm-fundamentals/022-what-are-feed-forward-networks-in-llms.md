# What are Feed-Forward Networks in LLMs?

**Topic:** LLM Fundamentals

## Source

- [Feed-Forward Networks in LLMs](https://outcomeschool.com/blog/feed-forward-networks-in-llms)

## Feed-Forward Networks

The Transformer feed-forward network is a per-token MLP applied after attention in each layer.

Key points:
- Attention mixes information across tokens; the FFN transforms each token representation independently.
- Modern FFNs often use gated activations such as SwiGLU and have a larger hidden dimension than the model dimension.
- A large share of Transformer parameters live in FFN layers.

## Example

Example: after attention gathers context for a token, the FFN transforms that token representation into higher-level features useful for the next layer.

## Current Software Engineering Use Case

Optimizing FFN kernels and quantizing FFN weights are common ways to reduce LLM serving cost.
