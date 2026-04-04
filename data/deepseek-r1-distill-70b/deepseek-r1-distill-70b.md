## Overview

DeepSeek R1 Distill 70B is a reasoning-focused model in the 70B parameter range, part of the DeepSeek R1 distill family. It uses knowledge distillation to compress reasoning capabilities from larger models into a more efficient 70B parameter form.

## Deployment

- **VRAM Requirements**: 24-48GB
- **Hardware**: Requires A100/H100 or multi-GPU consumer setup
- **Frameworks**: Compatible with Ollama, vLLM, llama.cpp, and Text Generation Inference
- **Quantization**: Supports GGUF quantization (Q4_K_M) to reduce VRAM by 50-75% with approximately 2% quality loss

## Capabilities

- Strong reasoning performance
- Open source license for self-hosting and fine-tuning