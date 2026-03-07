## Overview

Chronos is a family of pretrained time series forecasting models developed by Amazon Science. Based on language model architectures (T5 transformers), Chronos transforms time series into token sequences for training, enabling powerful zero-shot forecasting capabilities.

## How It Works

Chronos uses a novel approach to time series forecasting:

1. **Tokenization**: Time series are transformed into sequences of tokens via scaling and quantization
2. **Training**: A language model is trained on these tokens using cross-entropy loss
3. **Forecasting**: Probabilistic forecasts are obtained by sampling multiple future trajectories given historical context

## Model Variants

### Chronos-2 (Latest)
- **Parameters**: 120 million
- **Architecture**: Encoder-only time series foundation model
- **Release**: October 2025
- **Capabilities**: Univariate, multivariate, and covariate-informed forecasting in a single architecture
- **Performance**: State-of-the-art zero-shot accuracy among public models

### Chronos-Bolt
- **Accuracy**: 5% lower error than original Chronos
- **Speed**: Up to 250x faster than original Chronos
- **Memory**: 20x more memory efficient
- **Use Case**: Production deployments requiring high throughput

### Original Chronos
- **Architecture**: Based on T5 transformer models
- **Variants**: Multiple sizes (tiny, mini, small, base, large)
- **Foundation**: Established the tokenization approach for time series

## Benchmark Performance

### State-of-the-Art Results

Chronos-2 achieves state-of-the-art zero-shot accuracy on:
- **fev-bench**: Leading performance
- **GIFT-Eval**: Top scores among public models
- **Chronos Benchmark II**: Highest accuracy

### Adoption
- **600+ million downloads** from Hugging Face (Chronos and Chronos-Bolt combined)
- Widely adopted in industry and research

## Key Features

### Zero-Shot Forecasting
- No fine-tuning required on target datasets
- Generalizes across diverse time series domains
- Handles various frequencies and patterns

### Probabilistic Forecasts
- Generates multiple possible future trajectories
- Provides uncertainty quantification
- Supports risk-aware decision making

### Flexible Input Types
- Univariate time series (single variable)
- Multivariate time series (multiple related variables)
- Covariate-informed forecasting (using external factors)

## Use Cases

- Demand forecasting for retail and supply chain
- Financial market prediction
- Energy consumption forecasting
- Weather and climate predictions
- Server load and capacity planning
- Healthcare metrics forecasting
- IoT sensor data prediction

## Deployment Options

### Cloud Services
- **Amazon SageMaker JumpStart**: Deploy with just a few lines of code
- **AWS Integration**: Native support for AWS ecosystem

### Open Source
- **GitHub**: https://github.com/amazon-science/chronos-forecasting
- **Hugging Face**: Multiple model sizes available
  - amazon/chronos-2
  - amazon/chronos-t5-large
  - amazon/chronos-bolt-*

### Frameworks
- Compatible with standard PyTorch workflows
- Integration with time series libraries
- REST API deployment options

## Architecture Details

**Chronos-2** uses an encoder-only architecture optimized for:
- Efficient processing of time series sequences
- Support for variable-length inputs
- Handling missing values and irregular sampling
- Multi-task learning across forecast types

## Training Approach

Models are trained on:
- Diverse time series datasets from multiple domains
- Synthetic time series for improved generalization
- Real-world forecasting benchmarks
- Various temporal patterns and frequencies

## Licensing

Apache 2.0 license - open source for research and commercial use.

## Pricing

Free and open source. AWS deployment costs apply when using SageMaker or other AWS services.