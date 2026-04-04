## Overview

OpenAI's Moderation API is a content filtering service that detects potentially harmful categories in text inputs and outputs, enabling developers to block or flag policy-violating content before it reaches end users.

## Features

- **Multi-category detection**: Identifies hate speech, self-harm, sexual content, violence, illegal activity requests, and other harmful content types
- **Severity scoring**: Provides per-category risk scores allowing configurable threshold tuning
- **Input and output filtering**: Can be applied to both user prompts and model responses
- **Cloud-hosted API**: Fully managed by OpenAI with regular model updates
- **Integrated with base models**: GPT models themselves are alignment-trained (RLHF) to refuse harmful requests, with the Moderation API serving as an additional backstop

## Use Cases

- Content moderation for user-facing chatbots and generation endpoints
- Compliance filtering for enterprise deployments
- Automated content flagging for human review workflows

## Limitations

- Code-related queries may be misclassified as potential exploits
- Multilingual coverage remains a gap — non-English jailbreaks can bypass filters
- False positives occur for benign content containing trigger words

## Pricing

Free to use for standard moderation categories. No additional usage cost reported.