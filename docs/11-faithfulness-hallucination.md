# Intrinsic Faithfulness and Hallucination Evaluation

Factual consistency was evaluated separately from lexical and semantic similarity.

An XLM-RoBERTa-Large model fine-tuned on the Cross-Lingual Natural Language Inference (XNLI) benchmark was employed as an independent cross-lingual NLI evaluator.

For each source article and generated summary:

- The source article was treated as the premise.
- The generated summary was treated as the hypothesis.

The model predicts three inference classes:

- Entailment (E)
- Neutral (N)
- Contradiction (C)

## Intrinsic Evaluation

The proposed pipeline performs intrinsic evaluation of the generated summaries.

NLI predictions were obtained for the complete test set and were used to calculate faithfulness and hallucination measures.

## Faithfulness

For each evaluated record, faithfulness is calculated as:

\[
Faithfulness_i =
\frac{E_i}{E_i+N_i+C_i}
\]

A higher value indicates stronger alignment between the generated summary and the source article.

## Hallucination

The weighted hallucination measure is calculated as:

\[
Hallucination_i =
\frac{N_i+2C_i}{E_i+N_i+C_i}
\]

Neutral receives a weight of 1 because it represents uncertain or partial support.

Contradiction receives a weight of 2 because it represents information that directly conflicts with the source article and therefore represents a stronger form of factual inconsistency.

The formulation follows the NLI-based factual consistency evaluation paradigm used as the methodological basis in the study.
