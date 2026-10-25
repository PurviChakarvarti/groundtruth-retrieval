# groundtruth-retrieval
## Retrieval Evaluation & Regression Framework

GroundTruth is an evaluation-first benchmark for measuring whether changes to a retrieval system actually improve search quality.
The project uses public court opinions as a proxy for a legal research corpus and evaluates retrieval using a human-reviewed golden dataset.

## Core Question
When we change chunking, retrieval strategy, embeddings, or reranking, did search actually get better?
GroundTruth answers that question with measurable evidence.

## What It Evaluates

- Recall@K
- Mean Reciprocal Rank (MRR)
- nDCG
- Per-category retrieval performance
- Retrieval vs. generation failures
- Retrieval latency
- Regression detection in CI

## Experiments

The benchmark compares:

1. Different chunk sizes
2. Dense vs. hybrid retrieval
3. Reranking enabled vs. disabled

## Engineering Principle

A retrieval change is not considered an improvement unless it can be demonstrated with:

- an evaluation
- a measurable result
- a defensible tradeoff

## Disclaimer

This project uses public legal documents for research and educational purposes.

It is not a legal advice system and should not be used for legal decision-making.
