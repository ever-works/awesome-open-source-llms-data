## Overview

EmbeddingGemma-300M is a compact multilingual text embedding model developed by Google DeepMind, derived from the Gemma 3 foundation model. With just 300 million parameters, it is purpose-built for on-device deployment on laptops, tablets, and mobile devices while delivering strong performance across multilingual retrieval and semantic similarity tasks.

## Features

- **Multilingual coverage**: Trained on data spanning 100+ languages, supporting cross-lingual and multilingual retrieval, clustering, and classification
- **Compact and efficient**: Runs in under 200MB RAM with quantization; generates embeddings in less than 22ms on EdgeTPU, ideal for real-time and edge applications
- **Matryoshka Representation Learning (MRL)**: Supports output truncation from 768 → 512 → 256 → 128 dimensions, enabling flexible tradeoffs between storage and precision
- **Strong benchmark performance**: Rivals much larger models on MTEB benchmarks despite its compact size

## Usage Considerations

- EmbeddingGemma activations do not support float16; use float32 or bfloat16 as needed
- Maximum input length of 2048 tokens, sufficient for most retrieval tasks but shorter than some larger embedding models

## Deployment

- Available on Hugging Face
- Optimized for EdgeTPU and edge device deployment
- Suitable for mobile, laptop, and tablet inference