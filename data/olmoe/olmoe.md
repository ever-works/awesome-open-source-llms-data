## Overview

OLMoE is a fully open-source mixture-of-expert (MoE) language model developed jointly by the Allen Institute for AI (AI2) and Contextual AI. It represents a breakthrough as the first MoE model released with complete transparency: open data, code, evaluations, logs, and intermediate training checkpoints.

## Architecture

### Sparse MoE Design
- **Total Parameters**: 7 billion
- **Active Parameters**: 1 billion (per forward pass)
- **Expert Configuration**: 64 small unique experts, 8 activated per token
- **Base Architecture**: Decoder-only LLM with MoE transformer layers

### Efficiency Benefits
- 2x faster training than equivalent dense models
- 6-7x less compute than 7B dense models with comparable performance
- First model on the Pareto frontier of performance and size with full openness

## Training

### Scale and Infrastructure
- **Training Tokens**: 5.1 trillion tokens
- **Hardware**: 256 NVIDIA H100 Tensor Core GPUs
- **Duration**: 10 days
- **Framework**: PyTorch FSDP with mixed-precision training

### Training Data
- Built on DataComp-Baseline
- Incorporates lessons from AI2's Dolma dataset
- Carefully curated mixture for optimal performance
- Total training: ~5 trillion tokens

## Benchmark Performance

### Performance Leadership
- **Best in class**: Among models with less than 2B active parameters
- **Outperforms 7B models**: Despite using 6-7x less compute
- Consistently strong across diverse benchmarks

### Comparison with Dense Models
OLMoE-1B-7B achieves performance comparable to:
- 7B parameter dense models
- While using only 1B active parameters per token
- Significantly faster inference and lower memory usage

## Model Versions

### OLMoE-1B-7B (Base)
- Pretrained foundation model
- Suitable for fine-tuning on custom tasks
- Full MoE architecture

### OLMoE-1B-7B-Instruct
- Adapted through instruction tuning
- Additional preference tuning (DPO/similar)
- Ready for chat and assistant applications

## Open Source Commitment

OLMoE is truly open source with:
- **Open Data**: Complete training dataset details
- **Open Code**: Full training and inference code
- **Open Logs**: All training logs and metrics
- **Intermediate Checkpoints**: Snapshots throughout training
- **Evaluation Results**: Comprehensive benchmark data

This makes OLMoE the most transparent MoE model available.

## Integration Ecosystem

OLMoE has been integrated into major frameworks:
- **vLLM**: High-throughput serving
- **SGLang**: Structured generation
- **llama.cpp**: CPU inference
- **Transformers**: Hugging Face integration

## Use Cases

- Research on mixture-of-experts architectures
- Efficient deployment with limited compute budgets
- Fine-tuning for domain-specific applications
- Educational purposes and transparency studies
- Production deployments requiring cost efficiency

## Deployment Options

### Inference Platforms
- Hugging Face Hub
- vLLM for high-throughput serving
- SGLang for structured generation
- llama.cpp for CPU deployment
- Standard transformer frameworks

### Hardware Requirements
- Much lower than 7B dense models due to sparse activation
- Efficient inference on consumer GPUs
- CPU inference possible with llama.cpp

## Advantages of MoE Architecture

### Efficiency
- Only 1B of 7B parameters active per token
- Faster inference than dense 7B models
- Lower memory bandwidth requirements

### Performance
- Matches or exceeds dense 7B models
- Better performance-to-compute ratio
- Enables larger capacity with same active parameters

### Specialization
- Different experts can specialize in different patterns
- Improved handling of diverse input types
- Better generalization across domains

## Research Impact

OLMoE enables research into:
- MoE training dynamics
- Expert specialization patterns
- Efficient scaling strategies
- Routing mechanisms and expert utilization
- Comparison of MoE vs. dense architectures

## Licensing

Apache 2.0 license - fully open source with permissive commercial use.

## Pricing

Free and open source.