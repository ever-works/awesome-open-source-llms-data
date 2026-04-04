## Overview

gte-multilingual-base is the latest model in Alibaba Group's GTE (General Text Embedding) family. With 305 million parameters, it balances high-quality embeddings with efficient resource usage, and stands out for strong multilingual retrieval and comprehensive representation evaluation performance.

## Features

- **Multilingual support**: Covers more than 70 languages with reliable multilingual retrieval performance
- **Elastic dense embeddings**: Supports elastic output dense representations, optimizing storage and improving downstream task efficiency
- **Encoder-only transformer architecture**: Smaller and more resource-efficient than decoder-only models like gte-qwen2-1.5b-instruct; delivers 10x inference speed improvement
- **Sparse vectors**: Can generate both dense and sparse vector representations

## Usage Considerations

- Performance may vary for certain languages due to limited language data during contrastive pre-training
- Results in inconsistent performance across different language families

## Related Models

- gte-Qwen2-7B-instruct: A top-ranking model on the MTEB leaderboard
- gte-large-en-v1.5: Optimized for English with a max sequence length of 8192