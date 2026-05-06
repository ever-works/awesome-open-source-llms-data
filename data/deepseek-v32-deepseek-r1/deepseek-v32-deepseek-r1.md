## Overview

DeepSeek’s open source LLM family includes two complementary approaches: DeepSeek-V3 as a high-performance general-purpose model and DeepSeek-R1 as a reasoning-focused model.

## Features

- Mixture-of-experts architecture: Uses large total parameters with selective activation (e.g., 671B total, 37B active) to improve efficiency and scalability
- Reinforcement learning-driven reasoning: DeepSeek-R1 develops advanced reasoning behaviors such as chain-of-thought, self-reflection, and verification through RL
- Multi-stage training pipeline: Combines pretraining, supervised fine-tuning, and reinforcement learning to improve both general and reasoning capabilities
- Distillation into smaller models: Transfers reasoning capabilities from large models into smaller, more efficient variants
- Extended context support: Handles long inputs with context windows up to 128K tokens
- Efficient training and inference design: Includes innovations such as multi-token prediction and optimized training strategies to reduce compute cost

## Pricing

Free and open-source under the Apache 2.0 license.