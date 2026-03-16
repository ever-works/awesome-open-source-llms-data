## Overview

OpenAI GPT-5 is presented as a 'unified system' that employs an internal router to select the most appropriate model for a given request. Simple queries are handled by a fast 'main' model, while more complex problems are escalated to a 'thinking' model.

## Key Features

*   **Unified System:** Dynamically routes prompts to specialized internal models.
*   **General Intelligence:** Designed for broad applicability across various tasks.
*   **Multimodal Reasoning:** Although primarily text-focused, it is part of a system that can handle diverse request types.
*   **High Performance:** Achieves high scores in expert-level reasoning benchmarks like GPQA Diamond.

## Benchmarks

| Benchmark            | Score        | Ranking       | Max Context Window |
| :------------------- | :----------- | :------------ | :----------------- |
| LMArena Elo (Text)     | 1437         | Rank 4        | 400k Tokens        |
| GPQA Diamond         | ~89.4%       |               |                    |
| MMMU                 | -            |               |                    |

## Architecturall Influence

GPT-5 incorporates 'thinking' variants for highly formidable coding agents and shows architecturall influence from the 'thinking' meta, dynamically allocating GPU power to 'think harder' on difficult problems.