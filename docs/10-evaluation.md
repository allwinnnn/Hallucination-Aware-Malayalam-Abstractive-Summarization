# Evaluation Metrics

The generated summaries were evaluated using ROUGE-1, ROUGE-2, ROUGE-L, BLEU, and BERTScore.

All reported metric values are represented on a 0-100 percentage scale.

## ROUGE

ROUGE measures lexical overlap between generated and reference summaries.

- ROUGE-1 measures unigram overlap.
- ROUGE-2 measures bigram overlap.
- ROUGE-L is based on the longest common subsequence.

## BLEU

BLEU measures n-gram precision between generated summaries and reference summaries.

SacreBLEU was used for BLEU computation with tokenization disabled.

## BERTScore

BERTScore evaluates semantic similarity using contextual transformer representations.

The evaluation used:

`bert-base-multilingual-cased`

with Malayalam specified for the evaluation language.

ROUGE and BLEU primarily capture lexical overlap, whereas BERTScore captures contextual semantic similarity.

This distinction is relevant to abstractive summarization because generated summaries may preserve the meaning of the reference while using different lexical forms or sentence structures.
