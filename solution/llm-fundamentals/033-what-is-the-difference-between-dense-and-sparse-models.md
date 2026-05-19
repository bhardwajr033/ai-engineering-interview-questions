# What is the difference between dense and sparse models?

**Topic:** LLM Fundamentals

## Source

- [Mixture of Experts Explained](https://outcomeschool.com/blog/mixture-of-experts)

## Mixture of Experts

A Mixture of Experts model routes each token to a subset of expert feed-forward networks instead of activating every parameter.

Key points:
- Sparse activation increases total parameter capacity without proportional compute per token.
- A router chooses which experts process each token.
- MoE improves serving trade-offs but adds routing, load-balancing, and deployment complexity.

## Example

Example: an MoE model may activate only 2 of 16 experts per token, giving high capacity without using every parameter for every request.

## Current Software Engineering Use Case

Large-scale inference platforms use MoE models to deliver high quality while keeping per-token compute lower than equally large dense models.
