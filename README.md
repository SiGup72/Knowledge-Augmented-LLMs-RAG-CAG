# Knowledge-Augmented Large Language Models: RAG, CAG, and Emerging Approaches

## Overview
This research project investigates and compares different knowledge-augmentation approaches for Large Language Models (LLMs) in educational question answering.

## Research Objectives
To evaluate four architectures using the same base LLM and educational QA dataset:

1. LLM-only
2. Retrieval-Augmented Generation (RAG)
3. Cache-Augmented Generation (CAG)
4. Combined RAG + CAG

## Dataset
**CK-12 Textbook Question Answering (TQA)**

- [Hugging Face Dataset](https://huggingface.co/datasets/notefill/ck12-tqa-instruction)
- 13,675 cleaned text-only records.
- Training: 8,643
- Validation: 2,524
- Test: 2,508

## Base Model
Qwen2.5-7B-Instruct

## Evaluation Metrics
- Answer correctness
- Faithfulness
- Relevance
- Retrieval quality
- Response latency
- Token usage

## Project Structure
- `data/` – Dataset documentation and data access information.
- `notebooks/` – Research implementation notebooks.
- `results/` – Experimental results and visualizations.
- `models/` – Model-related configurations and artifacts.
- `docs/` – Research documentation.

## Current Progress
- [x] Dataset preparation
- [ ] Base LLM setup
- [ ] RAG implementation
- [ ] CAG implementation
- [ ] Combined RAG + CAG
- [ ] Evaluation and comparison

## Research Scope
The project focuses on comparing the quality, grounding, and efficiency trade-offs of different knowledge-augmentation architectures.