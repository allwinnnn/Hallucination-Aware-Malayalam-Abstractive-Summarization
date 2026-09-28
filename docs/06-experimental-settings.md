# Experimental Settings

Three experimental configurations were used for all four models.

## Zero-Shot

In the zero-shot configuration, the model receives the input article through the summarization prompt without task-specific supervised training.

## Few-Shot

In the few-shot configuration, two article-summary demonstration pairs are included in the prompt.

These examples provide additional task guidance and contextual information to the pretrained model.

## Fine-Tuning

In the supervised fine-tuning configuration, the pretrained models are adapted using the Malayalam article-summary training data.

A common training framework was maintained across the evaluated models, with adjustments made according to model architecture and computational requirements.

Validation loss was monitored during training.

An early stopping patience of five epochs was used across the fine-tuning experiments.

For fine-tuned mT5, the best checkpoint was obtained at the 12th epoch.
