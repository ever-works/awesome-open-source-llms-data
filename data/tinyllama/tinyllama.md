## Overview

TinyLlama is a compact 1.1B parameter language model pretrained on approximately 3 trillion tokens for about 3 epochs. Building on the architecture and tokenizer of Llama 2, TinyLlama leverages advances from the open-source community to achieve exceptional computational efficiency while maintaining strong performance.

## Architecture

- **Parameters**: 1.1 billion
- **Base Architecture**: LLaMA 2
- **Training Tokens**: ~3 trillion (3 epochs)
- **Tokenizer**: LLaMA 2 tokenizer

## Training Efficiency

### Throughput Performance
- **Training Speed**: 24,000 tokens per second per A100-40G GPU
- **Superior to competitors**: Significantly faster than Pythia-1.0B and MPT-1.3B

### GPU Hours Comparison (300B tokens)
- **TinyLlama-1.1B**: 3,456 A100 GPU hours
- **Pythia**: 4,830 A100 GPU hours
- **MPT-1.3B**: 7,920 A100 GPU hours

### Key Optimizations
- FlashAttention for efficient attention computation
- Lit-GPT framework integration
- Optimized training pipeline

## Benchmark Performance

### Commonsense Reasoning Tasks

Evaluated on:
- HellaSwag
- OpenBookQA
- WinoGrande
- ARC-Easy
- ARC-Challenge
- BoolQ
- PIQA

**Combined Average Score**: 52.99

### Performance vs. Baselines
- Outperforms OPT-1.3B on various downstream tasks
- Surpasses Pythia-1.4B across multiple benchmarks
- Demonstrates better problem-solving skills than existing models of comparable size

### Additional Evaluations
- **BIG-Bench Hard (BBH)**: Challenging reasoning tasks
- **DROP**: Math reasoning capabilities
- **HumanEval**: Programming and code generation

## Key Features

- Excellent performance-to-size ratio
- Compatible with LLaMA ecosystem and tools
- Fast inference on resource-constrained devices
- Strong commonsense reasoning
- Decent programming capabilities for its size

## Use Cases

- Edge deployment on mobile devices
- Rapid prototyping and experimentation
- Educational and research applications
- Resource-constrained environments
- On-device AI applications
- Chatbots and virtual assistants with limited compute

## Deployment Options

- Runs on consumer GPUs and CPUs
- Compatible with standard transformer frameworks
- Hugging Face Hub integration
- Suitable for quantization and optimization
- Low memory footprint enables broader deployment

## Available Versions

- **TinyLlama-1.1B**: Base pretrained model
- **TinyLlama-1.1B-Chat**: Instruction-tuned variant for conversational applications

## Training Data

Pretrained on diverse text corpora totaling ~3 trillion tokens across:
- Web text
- Books
- Code repositories
- Academic papers
- Wikipedia and other knowledge sources

## GitHub Repository

https://github.com/jzhang38/TinyLlama

## Licensing

Apache 2.0 license - open source with permissive commercial use.

## Pricing

Free and open source.