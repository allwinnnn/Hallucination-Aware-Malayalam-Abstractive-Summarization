# Faithful Abstractive Malayalam Summarization Using Multilingual Language Models

A comparative study of Malayalam-to-Malayalam abstractive summarization using multilingual language models under zero-shot, few-shot, and supervised fine-tuning configurations.

## Models

The study evaluates:

- mBART
- mT5
- BLOOMZ
- Sarvam

## Experimental Configurations

Each model is evaluated using:

1. Zero-shot prompting
2. Few-shot prompting
3. Supervised fine-tuning

## Evaluation

The generated summaries are evaluated using:

- ROUGE-1
- ROUGE-2
- ROUGE-L
- BLEU
- BERTScore

Factual consistency is additionally evaluated using an intrinsic Natural Language Inference approach based on XLM-RoBERTa-Large fine-tuned on XNLI.

## Dataset

The final Malayalam summarization corpus contains 9,698 article-summary pairs after preprocessing and filtering.

The corpus was constructed using Malayalam summarization resources including SocialSum and the AI4Bharat Indic Sentence Summarization dataset.

## Main Result

Fine-tuned mT5 achieved the strongest overall lexical-generation performance:

| Metric | Score |
|---|---:|
| ROUGE-1 | 4.21 |
| ROUGE-2 | 0.41 |
| ROUGE-L | 4.23 |
| BLEU | 18.48 |
| BERTScore | 78.06 |
| Faithfulness | 84.46% |
| Hallucination | 18.06% |

## Repository Scope

This repository contains the documentation, methodology, experimental configurations, evaluation results, and references associated with the study.

The repository intentionally does not contain the Python implementation.
