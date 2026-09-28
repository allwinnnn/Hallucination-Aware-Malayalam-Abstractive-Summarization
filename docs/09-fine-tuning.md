# Fine-Tuning

Supervised fine-tuning was performed to adapt the pretrained models to the Malayalam abstractive summarization task.

A unified training framework was used across the four models while accounting for differences in model architecture and computational requirements.

Validation loss was monitored during training and an early stopping patience of five epochs was applied.

The best-performing fine-tuned mT5 checkpoint was obtained at epoch 12.

## Fine-Tuned Results

| Model | ROUGE-1 | ROUGE-2 | ROUGE-L | BLEU | BERTScore |
|---|---:|---:|---:|---:|---:|
| mT5 | 4.21 | 0.41 | 4.23 | 18.48 | 78.06 |
| mBART | 4.00 | 0.27 | 4.05 | 17.20 | 77.86 |
| BLOOMZ | 3.80 | 0.74 | 3.84 | 7.89 | 69.46 |
| Sarvam | 1.59 | 0.00 | 1.58 | 0.35 | 69.81 |

Fine-tuned mT5 achieved the strongest ROUGE-1, ROUGE-L, and BLEU scores among the evaluated configurations.
