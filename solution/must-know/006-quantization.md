# Quantization

**Topic:** Must Know

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
