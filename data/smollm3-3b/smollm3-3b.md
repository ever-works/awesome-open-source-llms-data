## Overview

SmolLM3-3B is a fully open instruct and reasoning model from Hugging Face. At the 3B scale, it outperforms Llama-3.2-3B and Qwen2.5-3B, while staying competitive with many 4B-class alternatives (including Qwen3 and Gemma 3) across 12 popular LLM benchmarks.

## Architecture

- 3B parameters
- Dual-mode inference: /think and /no_think
- Trained to 64K context, stretchable to 128K with YaRN extrapolation
- Best performance in six main European languages

## Key Features

- **Dual-mode reasoning**: Supports /think and /no_think modes, allowing fast responses by default and only paying the reasoning cost when a request is genuinely hard
- **Long context window**: Trained to 64K tokens, can stretch to 128K with YaRN extrapolation — strong fit for long-running agent sessions
- **Fully open recipe**: Released under the Apache 2.0 license with detailed training notes, public data mixture, and architecture configurations — reduces guesswork for fine-tuning or building derivatives
- **High benchmark performance**: Published full engineering blueprint including architecture decisions, data mixture, and post-training methodology

## Benchmark Performance

- Outperforms Llama-3.2-3B and Qwen2.5-3B
- Competitive with many 4B-class alternatives including Qwen3 and Gemma 3
- Evaluated across 12 popular LLM benchmarks

## Limitations

- Multilingual coverage is narrower than some peers; works best in six main European languages. For broader global coverage, careful benchmarking is recommended

## Licensing

Released under the Apache 2.0 license with fully transparent training methodology, data mixtures, and configuration files.