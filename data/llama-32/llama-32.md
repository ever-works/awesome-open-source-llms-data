## Overview

Llama 3.2 is Meta's family of edge-optimized small language models designed for local deployment on consumer hardware including laptops, mobile phones, and IoT devices. The family includes 1B and 3B parameter text models.

## Model Variants

| Spec | 1B | 3B |
|------|-----|-----|
| Parameters | 1B | 3B |
| Context | 128K | 128K |
| MMLU | - | 63.4% |
| Tool Use (BFCL V2) | 25.7% | 67.0% |
| Speed (Q4) | 60+ tok/s | 40-60 tok/s |
| VRAM (Q4) | ~1GB | ~2GB |

## Features

- 128K context window across all sizes
- Strong tool calling and function execution via BFCL V2 benchmark (67.0% on 3B)
- Structured output support
- Q4 quantization performance: 60+ tok/s for 1B, 40-60 tok/s for 3B
- Optimized for mobile deployment (8GB VRAM devices)
- Outperforms Phi-3-mini on several tool-use benchmarks

## Hardware Requirements

- 3B model fits in ~2GB VRAM with Q4 quantization
- Runs on any 4GB+ GPU with quantization
- CPU-only viable at 3-6 tok/s with Q4 quantization
- Apple Silicon: baseline performance on M1 8GB with 3B model

## Use Cases

- Tool calling and agent workflows
- Structured data extraction
- Mobile AI assistants
- Edge deployment with low latency requirements
- Real-time applications requiring sub-100ms responses

## Deployment

```
ollama pull llama3.2:3b
ollama run llama3.2:3b
```

## Pricing

Free and open-weight under Meta's license agreement.