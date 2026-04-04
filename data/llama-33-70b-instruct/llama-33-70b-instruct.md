## Overview

Llama 3.3 70B Instruct is an improved 70B instruction-tuned model in the Llama 3.x line from Meta, featuring a 128k context window in community builds and broad tool and community support. It is optimized for high-quality general assistant applications.

## Architecture

- 70B parameter dense transformer
- 128k context window (in community builds)
- Instruction-tuned for conversational and agentic tasks

## Key Features

- High-quality conversational abilities across diverse topics
- Strong performance on reasoning and general chat tasks
- Broad ecosystem support with extensive tooling and integrations
- 128k context window enables processing of long documents
- Active community with fine-tuning recipes and third-party tools

## Use Cases

- High-quality general-purpose chat assistants
- Agentic workflows and tool use
- Customer-facing applications
- Long-document analysis with 128k context

## Deployment

- Ollama: `ollama run llama3.3:70b`
- Server deployment via vLLM or TGI
- VRAM requirements: ~40 GB (4-bit), ~75 GB (8-bit)
- Suitable for single 80 GB GPU server deployment

## Licensing

Licensed under the Llama Community License. Permissive for commercial use but with an Acceptable Use Policy that restricts certain deployment scenarios. Fine-tuning for commercial purposes is permitted. Users should review the full license text for compliance.

## Limitations

The community license includes use restrictions that must be reviewed before deployment. Model requires significant computational resources, particularly at full precision.