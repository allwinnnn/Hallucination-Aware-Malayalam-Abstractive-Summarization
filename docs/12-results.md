# Overall Results

The complete comparison of the evaluated configurations is provided below.

| Model | Setting | ROUGE-1 | ROUGE-2 | ROUGE-L | BLEU | BERTScore |
|---|---|---:|---:|---:|---:|---:|
| mT5 | Zero-shot | 0.03 | 0.00 | 0.03 | 0.03 | 76.82 |
| mT5 | Few-shot | 0.44 | 0.04 | 0.44 | 0.96 | 83.49 |
| mT5 | Fine-tuned | 4.21 | 0.41 | 4.23 | 18.48 | 78.06 |
| mBART | Zero-shot | 1.43 | 0.17 | 1.45 | 0.69 | 80.97 |
| mBART | Few-shot | 0.65 | 0.00 | 0.62 | 1.52 | 80.23 |
| mBART | Fine-tuned | 4.00 | 0.27 | 4.05 | 17.20 | 77.86 |
| BLOOMZ | Zero-shot | 1.37 | 0.00 | 1.37 | 1.07 | 79.58 |
| BLOOMZ | Few-shot | 1.00 | 0.00 | 1.00 | 0.02 | 77.38 |
| BLOOMZ | Fine-tuned | 3.80 | 0.74 | 3.84 | 7.89 | 69.46 |
| Sarvam | Zero-shot | 0.22 | 0.01 | 0.22 | 0.80 | 81.61 |
| Sarvam | Few-shot | 0.05 | 0.00 | 0.05 | 0.34 | 81.70 |
| Sarvam | Fine-tuned | 1.59 | 0.00 | 1.58 | 0.35 | 69.81 |

## Main Observation

Fine-tuned configurations show stronger lexical-generation scores than their corresponding zero-shot and few-shot configurations.

Fine-tuned mT5 produced the strongest overall ROUGE-1, ROUGE-L, and BLEU results.

Fine-tuned mBART produced comparable performance.

BLOOMZ achieved the highest ROUGE-2 score among the fine-tuned models.

BERTScore remained comparatively higher than the lexical metrics across several configurations, indicating that semantic similarity can remain substantial despite limited exact lexical overlap.
