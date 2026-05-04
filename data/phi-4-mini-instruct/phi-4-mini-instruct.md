## Overview

Phi-4-mini-instruct is a lightweight, instruction-tuned model from Microsoft's Phi-4 family. It is trained on a mix of high-quality synthetic data and carefully filtered public datasets, with a strong emphasis on reasoning-dense content.

## Features

- 3.8B parameters
- Reasoning and multilingual performance comparable to 7B-9B models
- Multilingual support: over 20 languages
- Long context window: native support for 128K tokens
- Production-friendly licensing: MIT license

## Use Cases

- Document analysis
- RAG (Retrieval-Augmented Generation)
- Agent traces
- Instruction following and reasoning tasks

## Considerations

- Limited factual knowledge: may produce inaccurate or outdated facts for knowledge-heavy or long-tail queries; suggest pairing with RAG or external tools
- Language performance varies: performance outside English can be uneven; benchmark non-English or low-resource languages before deployment
- Sensitive to prompt format: performs best with recommended chat and function-calling formats

## Prompt Format

For general conversation and instructions, use:
<|system|>Insert System Message<|end|><|user|>Insert User Message<|end|><|assistant|>