## Overview

MPT (MosaicML Pretrained Transformer) is a family of open-source, commercially usable LLMs released by MosaicML (now part of Databricks) in summer 2023. The models prioritize either quality (MPT-30B) or efficiency (MPT-7B).

## Model Variants

### MPT-7B
- **Parameters**: 7 billion
- **Training**: 1T tokens of text and code
- **Performance**: Matches LLaMA-7B quality
- **License**: Open source, commercial use allowed

### MPT-7B-8K
- **Context Length**: 8K tokens (extended)
- **Use Case**: Long-context applications

### MPT-30B
- **Parameters**: 30 billion
- **Training**: H100 GPUs
- **Deployment**: Fits on single A100-80GB (16-bit) or A100-40GB (8-bit)
- **Focus**: Quality at efficient scale

### Specialized Variants
- **MPT-7B-Instruct**: Instruction-tuned for following commands
- **MPT-30B-Instruct**: Larger instruction-tuned model
- **MPT-7B-Chat**: Conversational variant
- **MPT-30B-Chat**: Larger conversational model

## Key Innovations

### ALiBi (Attention with Linear Biases)
- Better handling of variable context lengths
- No fixed position embeddings
- Enables length extrapolation
- Improved efficiency

### Deployment Optimization
MPT-30B size specifically chosen to:
- Deploy on single GPU (1x A100-80GB in 16-bit)
- Or 1x A100-40GB in 8-bit precision
- Reduce infrastructure costs
- Simplify deployment

## Performance

MPT models offer:
- Quality matching larger proprietary models
- Efficient inference
- Commercial-friendly licensing
- Strong code generation
- Good instruction-following (instruct variants)

## Training Infrastructure

- Trained with MosaicML's efficient training stack
- Leveraged NVIDIA H100 GPUs for MPT-30B
- Optimized training recipes
- Production-grade infrastructure

## Deployment Options

### Inference Technologies
- **HuggingFace Pipelines**: Standard deployment
- **NVIDIA FasterTransformer**: Optimized inference
- **ONNX**: Cross-platform deployment
- **MosaicML Inference Service**: Managed hosting

### Cost-Effective Serving
MPT-30B-Instruct managed endpoint:
- **Price**: $0.005/1K tokens
- **Comparison**: 4-6X cheaper than OpenAI DaVinci
- **Managed**: No GPU procurement needed
- **Infrastructure**: Fully managed serving

## LLM Foundry

MosaicML provides complete training/inference tools:
- Training scripts and code
- Fine-tuning capabilities
- Evaluation frameworks
- Deployment instructions
- Integration with Composer framework

## Key Features

- **Commercial Use**: Fully open for commercial applications
- **ALiBi Attention**: Variable context length handling
- **Efficient Deployment**: Single-GPU inference
- **Multiple Sizes**: 7B and 30B variants
- **Specialized Versions**: Instruct and Chat variants
- **Complete Tooling**: Training and inference frameworks

## Use Cases

- **Enterprise Applications**: Commercial deployment
- **Cost-Sensitive Deployments**: Affordable serving
- **Custom Fine-Tuning**: Domain adaptation
- **Research**: Open model for experiments
- **Long-Context Tasks**: Extended context variants
- **Conversational AI**: Chat variants

## Training Efficiency

MPT demonstrates:
- Efficient training at scale
- Production-ready approaches
- Reproducible results
- Best practices for LLM training

## Community and Support

- Open-source codebase
- Active development and updates
- Databricks ecosystem integration
- Documentation and tutorials
- Community contributions

## Licensing

Apache 2.0 license allowing commercial use.

## Pricing

**Model Weights**: Free and open-source

**Managed Inference**: $0.005/1K tokens (competitive pricing)