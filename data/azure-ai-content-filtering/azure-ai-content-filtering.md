## Overview

Azure AI Content Filtering is Microsoft's built-in safety system for language model deployments on Azure, combining automated harm detection with Prompt Shield technology for defense against jailbreak and prompt injection attacks.

## Features

- **Harm categories**: Detects hate speech, violence, self-harm, sexual content, and other harmful categories
- **Prompt Shield**: Dedicated jailbreak detection for adversarial inputs targeting model instructions
- **Customizable severity thresholds**: Administrators can tune filtering strictness per harm category and per application
- **Groundedness detection**: Evaluates whether model responses are grounded in provided source material (for RAG scenarios)
- **Protected text detection**: Identifies and blocks copyrighted text in outputs
- **Integrated API and SDK**: Available through Azure AI Content Safety service with REST API and client SDKs
- **Monitoring and analytics**: Logging and metrics for tracking filter performance over time

## Use Cases

- Enterprise AI applications on Azure requiring compliance and safety
- Protected content generation needing copyright awareness
- RAG applications requiring groundedness verification

## Pricing

Included at no additional cost for text moderation with Azure OpenAI Service. Azure AI Content Safety offers tiered pricing for standalone use.