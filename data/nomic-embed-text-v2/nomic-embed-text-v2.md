## Overview

Nomic Embed Text V2 is a multilingual embedding model from Nomic AI and the first to use a Mixture-of-Experts (MoE) architecture for text embeddings. Trained on 1.6 billion contrastive pairs from mC4 and multilingual CC News across approximately 100 languages, it is designed for semantic search, RAG, and recommendation tasks.

## Architecture

- **Mixture-of-Experts (MoE)**: Alternating MoE layers with 8 experts and top-2 routing, activating only 305M out of 475M total parameters during inference
- **Dynamic routing**: Input is dynamically routed to only a subset of total parameters for optimal balance between performance and efficiency

## Features

- **Multilingual coverage**: Trained on ~100 languages from mC4 and multilingual CC News
- **High benchmark performance**: Strong results on BEIR and MIRACL benchmarks, competitive with models twice its size
- **Matryoshka Representation Learning**: Supports truncation from 768 to 256 dimensions while maintaining embedding quality
- **Fully open-source**: Pre-training and fine-tuning datasets, training code, and model weights are all open-sourced

## Usage Considerations

- Use structured input formats like `search_document: <text>` or `search_query: <text>` for optimal performance
- Maximum input length of 512 tokens
- Performance may vary across different languages, especially low-resource ones

## Deployment

- Available on Hugging Face
- Pre-training and fine-tuning code is open-source for customization
- Can be deployed with BentoML for scalable API serving