# Data Preprocessing

The source datasets were processed to create a consistent Malayalam article-summary corpus.

The article and summary fields required for the summarization task were extracted and standardized.

The following filtering operations were applied:

- Samples containing English words within the summaries were removed.
- Articles containing fewer than 30 characters were removed.
- Summaries containing fewer than 10 characters were removed.
- Very short summaries with insufficient content were therefore excluded.

After preprocessing and filtering, the final dataset contained 9,698 Malayalam article-summary pairs.

The processed corpus was subsequently divided into training, validation, and test sets.
