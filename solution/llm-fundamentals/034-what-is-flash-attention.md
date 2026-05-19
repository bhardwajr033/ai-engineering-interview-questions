# What is Flash Attention?

**Topic:** LLM Fundamentals

## Source

- [Decoding Flash Attention in LLMs](https://outcomeschool.com/blog/decoding-flash-attention)

## Flash Attention

Flash Attention is an IO-aware exact attention algorithm that reduces memory reads/writes by tiling attention computation.

Key points:
- It avoids materializing the full attention matrix in high-bandwidth memory.
- It improves speed and memory efficiency, especially for long sequences.
- It preserves exact attention results, unlike approximate sparse attention methods.

## Example

Example: a long-context training job can use Flash Attention to avoid storing the full attention matrix and fit larger batches on the same GPU.

## Current Software Engineering Use Case

Training and serving stacks use Flash Attention kernels to support longer contexts and higher throughput on GPUs.
