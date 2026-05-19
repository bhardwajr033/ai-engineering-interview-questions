# What is KV cache, and how do you manage memory for it?

**Topic:** AI Infrastructure and Scalability

## Source

- [What is KV Cache in LLMs?](https://outcomeschool.com/blog/kv-cache-in-llms)

## KV Cache

The KV cache stores key and value tensors for previous tokens so autoregressive decoding does not recompute them every step.

Key points:
- It speeds inference because each new token only needs attention against cached past keys and values.
- Memory grows with sequence length, batch size, layers, and number of KV heads.
- Paged attention manages KV memory in blocks to reduce fragmentation and support many concurrent requests.

## Example

Example: in a 50-turn chat, the server stores prior keys and values so each new token does not recompute the entire conversation.

## Current Software Engineering Use Case

LLM serving engines use KV caching and paged attention to support long chats, streaming responses, and continuous batching efficiently.
