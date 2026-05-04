## Overview

SmolLM3-3B is a fully open instruct and reasoning model from Hugging Face. At the 3B scale, it outperforms Llama-3.2-3B and Qwen2.5-3B, while staying competitive with many 4B-class alternatives (including Qwen3 and Gemma 3) across 12 popular LLM benchmarks.

## Features

- Dual-mode reasoning: supports /think and /no_think, so you can default to fast responses and only pay the reasoning cost when a request is genuinely hard
- Long context window: trained to 64K and can stretch to 128K tokens with YaRN extrapolation
- Fully open recipe: released under the Apache 2 license plus detailed training notes, public data mixture, and configs
- Transparency: full engineering blueprint published, including architecture decisions, data mixture, and post-training methodology

## Use Cases

- Long-running agent sessions
- Document analysis
- Reasoning-intensive tasks
- Instruction following

## Considerations

- Multilingual coverage is narrower than some peers: works best in six main European languages. If you need broader global coverage, benchmark carefully and consider alternatives.

## Recommendation

If you're building internal variants or want to understand what actually drives quality at 3B, the full transparency of SmolLM3-3B matters.