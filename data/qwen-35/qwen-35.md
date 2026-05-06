## Overview

Qwen 3.5 is a large-scale open-weight model designed as a native multimodal agent, combining vision and language capabilities within a unified architecture. It uses a hybrid design that mixes sparse mixture-of-experts with linear attention mechanisms to improve efficiency while maintaining strong performance. The model is trained on large multimodal datasets and supports long-context reasoning, tool use, and multilingual tasks.

## Features

- Hybrid MoE architecture: Combines sparse mixture-of-experts with linear attention to balance performance and inference efficiency
- Native multimodality: Integrates text and visual inputs through early fusion for cross-modal reasoning
- Large context window: Supports up to 1M tokens for long documents, conversations, and video inputs
- Agentic tool use: Includes built-in support for tool calling, search, and code execution within workflows
- Expanded multilingual support: Covers over 200 languages and dialects for global use cases
- Efficient inference design: Activates a small subset of parameters per request to reduce compute cost while maintaining capability

## Pricing

Free and open-source under the Apache 2.0 license (open variants).