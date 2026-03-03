## Overview

DeepHermes-3 is Nous Research's innovative "toggle-on reasoning" model, representing a new paradigm for LLMs that unify two opposing capabilities in a single model. The 8B variant enables efficient deployment while maintaining reasoning power.

## Dual Capabilities

### Traditional Mode
- Intuitive responses
- Fast generation
- Conversational style
- Immediate answers

### Reasoning Mode
- Extended chain of thought
- Deep problem analysis
- Step-by-step decomposition
- Improved accuracy

## Toggle Mechanism

- **Control**: System prompt switching
- **Flexibility**: Choose reasoning depth per query
- **Efficiency**: Fast when reasoning not needed
- **Quality**: Deep thinking when required

## Model Architecture

- **Base**: Llama 3.1 8B
- **Enhancement**: Instruction tuning for reasoning
- **Parameters**: 8 billion
- **Status**: Preview release

## Model Variants

**Available sizes:**
- 3B (Llama 3 based)
- 8B (Llama 3.1 based)
- 24B (Mistral based)

## Use Cases

- Task-dependent reasoning requirements
- Consumer-grade local deployment
- Research exploration
- Custom fine-tuning
- Inference optimization studies

## Performance

- Competitive with base Llama 3.1 8B
- Reasoning mode improves accuracy on complex tasks
- Efficient inference in both modes

## Licensing Considerations

Note: Not fully open-source in traditional sense. Organizations with 700M+ monthly active users require Meta's explicit approval for commercial use.

## Deployment

- Local inference on consumer hardware
- Cloud and on-premises options
- Quantization support
- Fine-tuning capabilities