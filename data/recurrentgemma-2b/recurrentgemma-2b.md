## Overview

RecurrentGemma is a family of open-weights language models from Google DeepMind based on the novel Griffin architecture. This represents a significant departure from transformer-only models, combining linear recurrences with local attention.

## Griffin Architecture Innovation

The Griffin architecture achieves:
- Fast inference on long sequences
- Fixed-sized state reducing memory use
- Efficient long-context generation
- Strong language understanding
- Excellent instruction-following

## Performance vs Traditional Transformers

Compared to Gemma-2B:
- Comparable task performance
- Lower memory requirements
- Faster inference on long sequences
- Trained on fewer tokens
- Better efficiency-to-performance ratio

## Model Variants

- **RecurrentGemma-2B**: Base pre-trained model
- **RecurrentGemma-2B-IT**: Instruction-tuned variant

## Technical Details

- Parameters: 2 billion
- Architecture: Griffin (linear recurrence + local attention)
- State Size: Fixed, enabling efficient long-context inference
- Training: High-quality curated data

## Use Cases

- Long document processing
- Streaming text generation
- Memory-constrained environments
- Mobile and edge deployment
- Real-time inference

## Memory Advantages

- Requires less memory than Gemma-2B
- Fixed state size enables better memory prediction
- Efficient for long context windows
- Better resource utilization

## Licensing

Open-weights model from Google DeepMind with permissive licensing for research and commercial use.