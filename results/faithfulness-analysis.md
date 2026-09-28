# Faithfulness and Hallucination Results

The intrinsic factual-consistency evaluation uses XLM-RoBERTa-Large fine-tuned on XNLI.

| Model | Approach | Faithfulness (%) | Hallucination (%) |
|---|---|---:|---:|
| mT5 | Zero-shot | 25.06 | 97.86 |
| mT5 | Few-shot | 37.65 | 92.45 |
| mT5 | Fine-tuned | 84.46 | 18.06 |
| mBART | Zero-shot | 68.10 | 39.77 |
| mBART | Few-shot | 44.33 | 63.86 |
| mBART | Fine-tuned | 79.45 | 24.00 |

The detailed intrinsic faithfulness and hallucination comparison was performed for mT5 and mBART.
