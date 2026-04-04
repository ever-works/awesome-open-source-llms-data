## Overview

Qwen 3.6 Plus was released on OpenRouter on March 31, 2026. It extends the Qwen family's lead with a 1M-token context window and a novel hybrid architecture combining linear attention mechanisms with sparse MoE.

## Architecture

- **Hybrid Architecture**: Combines linear attention with sparse MoE
- Linear attention reduces the computational cost of processing long sequences (overcoming the quadratic bottleneck in standard attention)
- Sparse MoE activates only the necessary experts per token
- Handles 1M tokens with significantly less compute than standard dense-attention models at comparable scale

## Key Features

- 1M-token context window
- Always-on chain-of-thought reasoning that reaches conclusions faster and uses fewer output tokens
- Reduced latency and cost on straightforward tasks
- Part of the broader Qwen family spanning 0.8B to 397B-A17B under Apache 2.0
- Strong performance on coding benchmarks (LiveCodeBench, SWE-bench)

## Benchmarks

- Leads on coding benchmarks (LiveCodeBench, SWE-bench) with clear margins over Llama 4 and Gemma 4
- Qwen 3.5 family delivers competitive performance at 10-17x lower cost than Claude or GPT for comparable tasks

## Pricing

Apache 2.0 license with a free preview period. Full parameter details and post-preview pricing TBD.

## Ecosystem

The broader Qwen 3.5/3.6 family covers more deployment scenarios under Apache 2.0 than any competitor — from Qwen 3.5 0.8B for edge devices to Qwen 3.5 397B-A17B for frontier tasks to Qwen 3.6 Plus for 1M-context workloads.