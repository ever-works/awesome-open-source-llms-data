## Overview
MiMo-V2-Flash is an A-tier open-source large language model from Xiaomi, known for its balanced performance across various tasks.

## Features
- **AIME 2025 Score:** 94.1.
- **GPQA Diamond Score:** 83.7.
- **Context Window:** 262K tokens.
- **HumanEval Performance:** 84.8.

## Best for
- Balanced coding and reasoning workloads
- High-throughput production serving

## Benchmarks
- MMLU: 86.7
- MMLU-Pro: 84.9
- HumanEval: 84.8
- SWE-bench Verified: 73.4
- LiveCodeBench: 80.6
- AIME 2025: 94.1
- GPQA Diamond: 83.7
- Chatbot Arena: 1401: ~150 tokens/second

## Benchmarks

| Benchmark | Score |
|-----------|------|
| AIME 2025 | 94.1% |
| SWE-Bench Verified | 73.4% |

## Cost Efficiency

- Operates at just 2.5% of Claude's inference cost while delivering comparable performance on specific reasoning tasks
- Fast inference at 150 t/s enables real-time applications

## Strengths

- Exceptional efficiency with 15B active parameters delivering strong math and coding performance
- Outstanding cost profile at 2.5% of Claude's inference cost
- Fast inference at 150 t/s enables real-time applications
- Strong mathematical reasoning with 94.1% AIME 2025 score
- Represents cutting-edge MoE efficiency techniques

## Weaknesses

- Instruction-following can be inconsistent on general-purpose tasks
- Performance strongest within math and coding domains, less reliable on diverse workloads
- Limited ecosystem maturity with sparse community tooling and documentation
- Best suited for narrow, well-defined use cases rather than general reasoning agents

## Primary Use Cases

- Mathematical competitions
- Coding challenges
- Cost-sensitive deployments
- Real-time applications requiring fast inference

## Licensing

Open-weight with commercial use permitted.