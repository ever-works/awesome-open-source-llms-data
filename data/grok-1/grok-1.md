## Overview

Grok-1 is a 314B parameter open-weight model released by xAI. It is a dense (non-MoE) base model that provides a powerful foundation for research and fine-tuning, published under the fully permissive Apache 2.0 license.

## Architecture

- Dense transformer architecture with 314B total parameters
- 78.5B active parameters per token (all parameters are active in dense mode)
- 8k context window

## Key Features

- Fully permissive Apache 2.0 license allowing commercial use, modification, and distribution
- Massive parameter scale suitable for research and advanced fine-tuning
- Open weights with no restrictive acceptable-use policies
- Strong reasoning capabilities as a pre-trained base model

## Use Cases

- Large-scale research projects
- Foundation model for custom fine-tuning
- Academic studies on large transformer behavior
- Enterprise customization with full license flexibility

## Deployment

- Not available on Ollama due to its large size
- Requires multi-GPU infrastructure for inference
- Compatible with vLLM and Hugging Face Text Generation Inference (TGI)
- VRAM requirements: ~180 GB (4-bit), ~320 GB (8-bit)

## Licensing

Licensed under Apache 2.0, fully permissive for commercial use including fine-tuning, modification, and distribution. This is one of the most permissive licenses available for a model of this scale.

## Limitations

Grok-1 is a base model, not an instruction-tuned variant, requiring significant fine-tuning to be useful for chat applications. Its immense size makes it impractical for all but the most well-resourced teams. The 8k context window is smaller than many modern alternatives.