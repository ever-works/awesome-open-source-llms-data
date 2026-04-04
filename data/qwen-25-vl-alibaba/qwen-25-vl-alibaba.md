## Overview

Qwen 2.5 VL is a flagship open-source vision-language model from Alibaba, available in sizes ranging from 3B to 72B parameters. The 72B model rivals GPT-4o in document understanding benchmarks. It achieves competitive scores including MMBench >80% and MM-Vet >75%.

## Technical Details

- **Model sizes**: 3B, 7B, 72B parameters
- **Vision Encoder**: Custom Vision Transformer (ViT) with Native Dynamic Resolution
- **Language Backbone**: Qwen LLM
- **Context Window**: 128k tokens
- **Video Support**: Up to 1 hour of video with Absolute Time Encoding for precise event localization
- **Languages**: Support for 29 languages
- **Key Innovations**: Dynamic resolution ViT handles diverse image sizes without normalization; structured data extraction; object localization; agentic capabilities

## Features

- **Native Dynamic Resolution**: Processes images and videos of various sizes without normalization
- **Absolute Time Encoding**: Enables precise video event localization for temporal understanding
- **Object Localization**: Excels at identifying and localizing objects within images
- **Multilingual OCR**: Supports optical character recognition across 29 languages
- **Long Video Understanding**: Processes up to one hour of video content
- **Structured Data Extraction**: Extracts structured data from documents and diagrams
- **Agentic Capabilities**: Can interact with digital environments and perform automated tasks
- **Document Understanding**: Rivals GPT-4o in document and diagram comprehension

## Use Cases

- Automated data entry from scanned documents and forms
- Interactive UI agents for user interface automation
- Long video analysis and indexing with timestamp precision
- Multilingual OCR for international document processing
- Log shipping manifest processing and container detail extraction
- Edtech platforms for lecture video indexing and search

## Licensing

Released under the Apache 2.0 license, allowing free commercial and research use.