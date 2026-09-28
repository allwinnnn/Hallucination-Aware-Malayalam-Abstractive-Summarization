# Few-Shot Results

The few-shot configuration introduces two article-summary examples into the prompt.

The inclusion of demonstrations provides additional task-specific guidance compared with zero-shot inference.

Among the few-shot configurations, mT5 obtained the highest BERTScore of 83.49%.

However, the improvements in ROUGE and BLEU remained limited.

This indicates that a small number of demonstrations can provide additional contextual guidance but does not provide the same degree of task-specific adaptation achieved through supervised fine-tuning.
