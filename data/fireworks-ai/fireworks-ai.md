## Overview

Fireworks AI is an inference platform designed for serving open-source language models at production scale. All seven models featured in the Fireworks best open-source LLMs roundup are available on the platform for immediate use.

## Performance

- 3-12x lower latency compared to vLLM
- 6-40x higher throughput compared to vLLM
- Processes over 300 billion tokens per day
- 100+ hosted models
- Handwritten CUDA kernels, distributed inference, semantic caching, and fine-grained quantization
- Immediate support for new model releases

## Deployment Options

| Option | How It Works | Best For |
|--------|-------------|----------|
| Serverless | Pay per token, no cold boots, 1 line of code | Prototyping and variable workloads |
| On-Demand | Private GPUs, ~250% better throughput vs vLLM, auto-scaling | Production workloads with predictable traffic |
| Enterprise Reserved | Dedicated GPUs, SLAs, priority support, bring-your-own-cloud | High-volume production with compliance requirements |

## API Compatibility

- OpenAI-compatible API; switching from GPT-4 to models like DeepSeek v3.2 or Kimi K2 requires changing one line of code
- Speculative Decoding API for accelerated inference

## Use Cases

- Cursor achieved 2x faster inference than GPT-4 with 30% fewer code errors and 1,000 tokens/second throughput
- Notion reduced latency from 2 seconds to 350 milliseconds with a fine-tuned 8B model
- Vercel improved code compilation rates from 62% to "way into the 90s" using reinforcement learning fine-tuning

## Pricing

- New users receive $1 in free serverless inference credits
- Serverless: pay-per-token pricing with no cold starts
- $1/hour for 100 tokens/second on specific model APIs (e.g., MiniMax-M2.5 standard tier)
- On-Demand and Enterprise Reserved plans available for production workloads