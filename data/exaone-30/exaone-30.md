## Overview

EXAONE 3.0 (EXpert AI for EveryONE) is Korea's first open-weights large language model, developed by LG AI Research. Released in August 2024 as open source for research purposes, it represents a significant milestone in Korean AI development with strong bilingual capabilities in Korean and English.

## Model Variants

### EXAONE 3.0 7.8B
- **Parameters**: 7.8 billion
- **Training Tokens**: 8 trillion
- **Languages**: Korean and English (bilingual)
- **Version**: Instruction-tuned for research purposes

### EXAONE 3.5
- Updated version released in late 2024
- Enhanced performance and capabilities

### K-EXAONE
- **Architecture**: Mixture-of-Experts
- **Total Parameters**: 236 billion
- **Active Parameters**: 23 billion (during inference)
- **Languages**: Multilingual (Korean, English, Spanish, German, Japanese, Vietnamese)

### Exaone Deep
- **Variant**: Exaone Deep-32B
- **Specialty**: Reasoning AI model
- **Release**: March 2025 as open source

## Benchmark Performance

### EXAONE 3.0 7.8B Real-World Benchmarks

**English:**
- MT-Bench: **Top score** in category
- Arena-Hard: **Top score** in category
- WildBench: **Top score** in category

**Korean:**
- Real-world scenarios: **Ranked 1st**
- General language understanding: **Ranked 1st**

### Exaone Deep-32B Performance
- Korean CSAT Math: **94.5** (2026 exam)
- MATH-500: **95.7** (mathematical problem-solving)

## Performance Improvements

Compared to predecessor models:
- **56% reduction** in inference time
- **35% decrease** in memory usage
- **72% reduction** in operational costs

## Architecture

K-EXAONE uses a Mixture-of-Experts (MoE) architecture that activates only a subset of parameters during inference, enabling:
- Efficient processing with reduced computational requirements
- Strong multilingual capabilities across 6 languages
- Balanced performance across different language families

## Training Data

EXAONE models are trained on massive multilingual datasets with particular emphasis on:
- Korean language corpora
- English language data
- Technical and scientific content
- Code and programming examples

## Capabilities

- Bilingual/multilingual text generation
- Real-world conversation and assistance
- Mathematical reasoning and problem-solving
- Code generation and understanding
- Complex reasoning tasks
- Korean-specific language understanding

## Deployment Options

- Hugging Face Hub (https://huggingface.co/LGAI-EXAONE)
- GitHub repository (https://github.com/LG-AI-EXAONE/K-EXAONE)
- LG Cloud platforms
- Standard transformer frameworks

## Licensing

Open source for research purposes. Check model-specific licenses on Hugging Face for commercial use terms.

## Pricing

Free for research purposes. Commercial licensing may vary by model variant.