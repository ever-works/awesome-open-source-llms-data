## Overview

NVIDIA Nemotron 3 is a family of open-source foundation models delivering leading efficiency and accuracy for building specialized AI agents with reasoning capabilities. Released in early 2026, the family includes models in Nano, Super, and Ultra sizes with breakthrough hybrid mixture-of-experts architecture.

## Model Variants

### Nemotron 3 Nano
- **Total Parameters**: 30B
- **Active Parameters**: 3B
- **Architecture**: Hybrid Mixture-of-Experts (23 Mamba-2 and MoE layers + 6 Attention layers)
- **Performance**: 4x higher throughput than Nemotron 2 Nano
- **Availability**: Available now on Hugging Face and inference providers
- **Context Window**: Up to 1 million tokens for agentic workflows

### Nemotron 3 Super
- **Total Parameters**: ~100B
- **Active Parameters**: ~10B
- **Use Case**: Multi-agent collaboration and low-latency reasoning
- **Availability**: Expected H1 2026

### Nemotron 3 Ultra
- **Total Parameters**: ~500B
- **Active Parameters**: ~50B
- **Use Case**: Large-scale reasoning engine for complex planning and research workflows
- **Availability**: Expected H1 2026

## Architecture

Nemotron-3-Nano uses a breakthrough hybrid mixture-of-experts architecture consisting of:
- 23 Mamba-2 and MoE layers
- 6 Attention layers
- Unified model for both reasoning and non-reasoning tasks

This architecture delivers the most tokens per second for multi-agent systems at scale.

## Additional Model Family (January 2026)

**Nemotron Speech**: Leaderboard-topping open models including ASR models for real-time, low-latency speech recognition

**Nemotron Multimodal RAG**: Models optimized for retrieval-augmented generation with multimodal inputs

**Nemotron Safety**: Specialized models for AI safety applications

## Deployment Options

### Inference Providers
- Baseten
- DeepInfra
- Fireworks
- FriendliAI
- OpenRouter
- Together AI

### Platforms
- Hugging Face Hub
- NVIDIA NIM for optimized deployment

## Open Source Commitment

NVIDIA publishes:
- Complete training datasets
- Training techniques and recipes
- Model weights
- Training logs and checkpoints

This allows the open-source community to learn from NVIDIA's approach and create derivative models.

## Licensing

NVIDIA Open Model License - a permissive license allowing users to use, modify, distribute, and commercially deploy models and derivatives without crediting NVIDIA.

## Pricing

Free and open source. Commercial deployment allowed without licensing fees.