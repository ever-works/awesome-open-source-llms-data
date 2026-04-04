## Overview

Llama Guard is an open-source family of content moderation models developed by Meta, optimized for detecting unsafe or policy-violating content in both user inputs and model outputs for LLM applications.

## Features

- **Distilled models**: Available in compact sizes (e.g., 7B parameters) suitable for local deployment
- **Content moderation**: Detects categories including hate speech, violence, self-harm, sexual content, illegal activities, and PII
- **Input and output filtering**: Can be applied to both prompts sent to the LLM and responses returned
- **Self-hosted**: Designed to run locally without cloud dependencies, enabling on-premises and air-gapped deployments
- **Quantization support**: Can be compressed to 8-bit or 4-bit precision for efficient inference on CPUs or small GPUs
- **Customizable**: Models can be fine-tuned on organization-specific policy guidelines

## Use Cases

- On-premises LLM deployments requiring local safety filtering
- Privacy-sensitive applications (GDPR, HIPAA compliance) where data must not leave the environment
- Edge deployments with resource constraints

## Pricing

Free and open-source under Meta's Llama Community License.