## Overview

Amazon Bedrock Guardrails is a managed safety service that integrates with Amazon Bedrock's model invocation pipeline to enforce content policies, detect sensitive information, and block topics that violate organizational requirements.

## Features

- **Denied topics**: Define entire categories that an application should avoid (e.g., medical advice, financial recommendations)
- **Custom word filters**: Block specific words or phrases tailored to business needs (slurs, competitor names, internal restricted terms)
- **PII/sensitive information filters**: Automatically detect personal data (emails, SSNs, etc.) and either block or redact it in outputs
- **Configurable sensitivity thresholds**: Tune content category severity levels independently (e.g., decide whether mild profanity is acceptable)
- **Sub-second latency**: Deterministic policy checks operate in under a second
- **Integrated with Bedrock**: Intercepts calls within the AWS Bedrock service fabric, no separate network round-trip needed

## Use Cases

- Enterprise applications on AWS requiring compliance with internal policies
- Customer-facing chatbots needing PII protection
- Applications in regulated industries (finance, healthcare) requiring topic restrictions

## Pricing

Priced per text moderation request as part of Amazon Bedrock's usage-based pricing model. See AWS pricing pages for current rates.