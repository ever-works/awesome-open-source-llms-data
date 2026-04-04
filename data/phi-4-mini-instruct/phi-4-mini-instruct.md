## Overview

Phi-4-mini-instruct is a lightweight, instruction-tuned model from Microsoft's Phi-4 family. It is trained on a mix of high-quality synthetic data and carefully filtered public datasets, with a strong emphasis on reasoning-dense content.

## Architecture

- 3.8B parameters
- Trained on high-quality synthetic data and carefully filtered public datasets
- Strong emphasis on reasoning-dense content
- Instruct-tuned variant of the Phi-4 family

## Key Features

- **Multilingual support out of the box**: Supports over 20 languages, suitable for global products requiring lightweight multilingual capability
- **Long context window**: Native support for 128K tokens, usable in document analysis, RAG, and agent trace scenarios
- **Production-friendly licensing**: Released under the MIT license — freely usable, fine-tunable, and deployable in commercial systems without restrictive terms
- **Reasoning performance comparable to larger models**: Shows reasoning and multilingual performance comparable to models in the 7B–9B range such as Llama-3.1-8B-Instruct

## Limitations

- **Limited factual knowledge**: Does not store large amounts of world knowledge; may produce inaccurate or outdated facts for knowledge-heavy or long-tail queries. Best paired with RAG or external tools for production use
- **Uneven non-English performance**: Performance outside English can vary; non-English or low-resource languages should be carefully benchmarked before deployment
- **Sensitive to prompt format**: Performs best with recommended chat and function-calling formats. Deviations can negatively impact instruction adherence and output quality

## Prompt Format

For general conversation and instructions, the recommended format is:
```
<|system|>Insert System Message<|end|><|user|>Insert User Message<|end|><|assistant|>
```

## Licensing

Released under the MIT license — fully open for commercial use, fine-tuning, and deployment.

## Deployment

At 3.8B parameters, it runs without the operational overhead of larger models, suitable for single-GPU deployments.