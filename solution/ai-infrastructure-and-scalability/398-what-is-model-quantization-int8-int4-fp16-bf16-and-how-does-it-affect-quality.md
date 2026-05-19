# What is model quantization (INT8, INT4, FP16, BF16), and how does it affect quality?

**Topic:** AI Infrastructure and Scalability

## Source

- [AI Engineering Explained: LLM, RAG, MCP, Agent, Fine-Tuning, Quantization](https://www.youtube.com/watch?v=lnfWvX66FUk)
  - Transcript notes: the video frames AI engineering around six practical building blocks: LLMs for language generation, RAG for grounding answers in external knowledge, MCP for standardized tool/data integration, agents for goal-directed tool use, fine-tuning for behavior or domain adaptation, and quantization for cheaper deployment.

## Quantization

Quantization stores or computes model weights/activations with lower precision to reduce memory, bandwidth, and cost.

Key points:
- FP16/BF16 are common training and inference formats; INT8 and INT4 reduce memory further.
- Post-training quantization is simpler; quantization-aware training can preserve more quality.
- Quality drops when precision is too low for sensitive layers or calibration data is poor.

## Example

Example: quantizing a 7B model from FP16 to INT4 can make local or edge inference feasible, but you must retest accuracy on real tasks.

## Current Software Engineering Use Case

Serving teams quantize LLMs to fit larger models on available GPUs, increase throughput, or run models on edge devices.
