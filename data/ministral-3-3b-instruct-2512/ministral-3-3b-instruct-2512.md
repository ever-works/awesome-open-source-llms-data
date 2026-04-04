## Overview

Ministral-3-3B-Instruct-2512 is a multimodal small language model developed by Mistral AI. It is the smallest instruct model in the Ministral 3 family, designed specifically for edge and resource-constrained deployments.

## Architecture

- 3.4B language model with 0.4B vision encoder
- Supports basic visual understanding alongside chat and instruction following
- Runs on a single GPU, fitting into roughly 8 GB of VRAM in FP8 (less with further quantization)
- Supports up to 256K token context

## Key Features

- **Vision + text in one small model**: Practical for lightweight image tasks like screenshot understanding, image captioning, and simple visual Q&A without moving to a large vision-language model
- **Agent-ready**: Designed with function calling and structured (JSON-style) outputs for easy integration into tool-using and agentic workflows
- **Large context for its size**: Up to 256K tokens supports document-heavy prompts, long logs, or multi-file inputs

## Limitations

- Visual reasoning capability is limited; best used for simple descriptions and basic Q&A rather than detailed image analysis or complex visual reasoning
- For stronger multimodal reasoning, the Ministral-3-3B-Reasoning-2512 variant is recommended

## Deployment

Runs on a single GPU with approximately 8 GB VRAM in FP8 precision, making it accessible for edge and resource-constrained environments. Further quantization can reduce memory requirements.