## Overview

Kimi K2 Thinking is a trillion-parameter Mixture-of-Experts model designed specifically for deep reasoning and tool use. The model is fully agentic and always thinks first — every output includes internal reasoning content by default.

## Architecture

- **Type**: Large-scale MoE
- **Total Parameters**: ~1T
- **Active Parameters**: ~32B per token
- **Experts**: 384
- **Context Length**: 256K native, up to ~1M with Yarn scaling
- **Training**: INT4 precision (natively), delivering up to 2x faster inference

## Thinking Mode

Kimi K2-Thinking only supports thinking mode, where the system prompt automatically inserts a <think> tag. Every output includes internal reasoning content by default.

## Benchmarks

| Benchmark | Score |
|-----------|------|
| Humanity's Last Exam | 44.9% |
| BrowseComp | 60.2% |
| Seal-0 (real-world information collection) | 56.3% |
| SWE-Multilingual | 61.1% |
| SWE-bench Verified | 71.3% |
| LiveCodeBench V6 | 83.1% |

Outperforms GPT-5 and Claude Sonnet 4.5 across reasoning, agentic, and coding evaluations.

## Strengths

- Excellent long-horizon reasoning
- Very large context window (256K native, 1M with Yarn)
- Strong tool-use and planning capability
- Efficient inference relative to total size (INT4 precision)

## Weaknesses

- Truly enormous scale (~1T) means daunting training/inference overhead
- Still early release, so real-world adoption and tooling is nascent

## Primary Use Cases

- Deep reasoning and complex problem-solving
- Planning and strategic analysis
- Long-context agents
- Tool-interactive workflows

## Licensing

Open-weight with commercial use permitted.