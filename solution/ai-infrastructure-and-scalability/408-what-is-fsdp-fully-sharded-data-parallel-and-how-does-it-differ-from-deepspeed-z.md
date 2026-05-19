# What is FSDP (Fully Sharded Data Parallel), and how does it differ from DeepSpeed ZeRO?

**Topic:** AI Infrastructure and Scalability

## AI Infrastructure

AI infrastructure focuses on serving or training models reliably under GPU, memory, latency, and cost constraints.

Key points:
- Parallelism splits work across devices: data parallelism splits batches, tensor parallelism splits matrix operations, and pipeline parallelism splits layers.
- Serving optimizations include KV cache, continuous batching, speculative decoding, quantization, model routing, request queues, and autoscaling.
- Monitoring should track time to first token, inter-token latency, throughput, queue time, GPU utilization, memory, errors, and cost.

## Example

Example: a chat service combines continuous batching, KV-cache management, autoscaling, and model routing to keep p95 latency stable.

## Current Software Engineering Use Case

A high-traffic chat platform uses batching, routing, GPU autoscaling, and backpressure to keep latency stable during traffic spikes.
