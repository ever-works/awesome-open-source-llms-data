## Overview

Ministral-3-3B-Instruct-2512 is a multimodal SLM developed by Mistral AI. It’s the smallest instruct model in the Ministral 3 family, designed specifically for edge and resource-constrained deployments.

## Features

- Combines a 3.4B language model with a 0.4B vision encoder
- Supports basic visual understanding alongside chat and instruction following
- Can run on a single GPU
- Fits into roughly 8 GB of VRAM in FP8, or even less with further quantization
- Supports up to 256k tokens context
- Designed with function calling and structured (JSON-style) outputs in mind

## Use Cases

- Lightweight image tasks: screenshot understanding, image captioning, simple visual Q&A
- Tool-using and agentic workflows
- Document-heavy prompts, long logs, or multi-file inputs

## Considerations

- Vision is functional, not deep: visual reasoning capability is limited
- Suggested for simple descriptions and basic Q&A rather than detailed image analysis or complex visual reasoning
- For stronger multimodal reasoning, consider Ministral-3-3B-Reasoning-2512 instead