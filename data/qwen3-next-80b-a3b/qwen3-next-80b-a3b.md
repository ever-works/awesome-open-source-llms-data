## Overview

Qwen3-Next is Alibaba's next-gen open model series emphasizing both scale and efficiency. The 80B-A3B-Thinking variant is specially designed for complex reasoning with a striking efficiency profile: 80B total parameters but only ~3B active.

## Architecture

- **Type**: Hybrid MoE with hybrid attention (linearized + sparse mechanisms)
- **Total Parameters**: 80B
- **Active Parameters**: ~3B (512 experts with 10 active)
- **Layers**: 48
- **Layout**: Hybrid
- **Native Context**: 262K tokens
- **Training**: Multi-token prediction (MTP) for speed

## Benchmarks

| Benchmark | Score |
|-----------|------|
| AIME25 (math) | ~87.8% |
| HMMT25 | ~73.9% |
| MMLU | Strong performance |
| Coding benchmarks | Strong performance |

Outperforms Gemini-2.5-Flash (72.0% on AIME25, 73.9% on HMMT25) on several benchmarks, and surpasses earlier Qwen-30B and Qwen-32B thinking models.

## Features

- Thinking mode: automatically generates <think> block
- 10x speedup for contexts over 32K compared to older Qwens
- Excellent reasoning and coding performance per compute
- Large native context window

## Strengths

- Excellent reasoning and coding performance per compute — beats larger models on many tasks
- Huge native context (262K)
- Extremely efficient — 10x speedup for >32K context vs older Qwens
- Fully Apache-2.0 licensed

## Weaknesses

- May require specific MoE runtime support
- Thinking mode adds complexity — always generates a <think> block and requires specific prompting
- Documentation primarily in Chinese with English materials still developing

## Licensing

Fully Apache-2.0 licensed.