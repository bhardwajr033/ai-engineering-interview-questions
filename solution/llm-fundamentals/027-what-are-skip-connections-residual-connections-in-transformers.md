# What are skip connections (residual connections) in Transformers?

**Topic:** LLM Fundamentals

## Source

- [Skip connections (residual connections) in Transformers](https://www.linkedin.com/posts/amit-shekhar-iitbhu_machinelearning-llm-deeplearning-share-7414239846707392512-pQdQ)

## Residual Connections

Residual connections add a layer input back to its output so information and gradients can flow through deep networks.

Key points:
- They make very deep Transformers easier to train.
- They preserve useful lower-level representations while layers add refinements.
- They work with normalization to stabilize optimization.

## Example

Example: a Transformer layer can add new context while the residual path preserves the original token representation for later layers.

## Current Software Engineering Use Case

Residual pathways are one reason production LLMs can scale to dozens or hundreds of layers without training collapse.
