## Overview

Nemotron 3 Nano is Nvidia's most efficient model, designed for edge, PC, and low-latency agent tasks.

## Specifications

| Attribute | Value |
|---|---|
| Parameters | 31.6B total / 3.6B active (MoE) |
| Context Window | 1,000,000 tokens |
| Knowledge Cutoff | Jun 2025 |

## Features

- 4x faster throughput than Nemotron 2 Nano
- Outperforms Qwen3-30B-A3B-Thinking on coding, reasoning, and math at 3.3x higher throughput
- Hybrid Mamba-2/Transformer architecture handles 1M tokens without quadratic attention cost
- Deployable on A100 or H100; quantized versions fit in 20-32GB VRAM
- Ideal for edge, PC, and low-latency agent tasks

## License

NVIDIA Open Model License