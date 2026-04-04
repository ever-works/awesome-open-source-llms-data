## Overview

Jina Embeddings v4 is a universal, multimodal, and multilingual embedding model developed by Jina AI, built on the Qwen2.5-VL-3B-Instruct foundation model. It is designed for complex retrieval scenarios that involve not only text but also images and visual documents such as charts, tables, or scanned pages.

## Features

- **Multilingual support**: Covers over 30 languages, including technical and visually complex documents
- **Unified multimodal architecture**: Single model for text, image, and code retrieval, eliminating the need for separate pipelines
- **Flexible embedding types**: Offers both dense (2048-dim) and multi-vector representations with Matryoshka support for dimensionality reduction down to 128, 256, etc.
- **Task-specific adapters**: Specialized adapters for retrieval, text matching, and code-related tasks, dynamically selected at inference time

## Licensing

- Released under CC-BY-NC-4.0 license, restricting direct commercial usage
- Commercial applications require using Jina's managed API or contacting the team

## Usage Considerations

- The model uses different adapters for tasks like code and retrieval, requiring awareness during integration
- Non-commercial license limits direct commercial deployment