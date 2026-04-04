## Overview

all-mpnet-base-v2 is a sentence embedding model based on MPNet, a pre-training method that addresses limitations of masked language modeling (MLM) in BERT and permuted language modeling (PLM) in XLNet. It uses a contrastive learning objective to map sentences and paragraphs into a 768-dimensional dense vector space and is one of the most downloaded embedding models on Hugging Face.

## Features

- **Extensive training**: Trained on over 1 billion sentence pairs to capture fine-grained semantic relationships
- **Highly adaptable**: Supports fine-tuning for specific tasks with 149 fine-tuned versions available on Hugging Face
- **768-dimensional output**: Ideal for clustering, semantic search, and other NLP tasks
- **Apache 2.0 license**: Supports both personal and commercial use under the license terms

## Usage Considerations

- Default input truncation at 384 word pieces, which may lead to context loss for longer text
- Moderate benchmark performance: does not rank particularly high on the MTEB leaderboard for certain tasks

## Related Models

- all-MiniLM-L6-v2 is a similar sentence-transformers model and a good starting point for beginners
- The BentoML deployment example in the source uses a similar model (all-MiniLM-L6-v2) for scalable serving