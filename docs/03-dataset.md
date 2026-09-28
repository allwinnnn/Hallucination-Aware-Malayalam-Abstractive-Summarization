# Dataset

## Dataset Sources

The final Malayalam summarization corpus was constructed using two publicly available resources.

### SocialSum Malayalam

The SocialSum Malayalam summarization dataset was sourced from Hugging Face and was released in 2024.

### AI4Bharat Indic Sentence Summarization

The AI4Bharat Indic Sentence Summarization dataset was sourced from Hugging Face and was released in 2022.

## Corpus Construction

The required article and summary fields were selectively extracted from the source datasets.

The article was used as the input and the corresponding Malayalam summary was used as the reference summary.

The extracted fields were standardized and merged to construct a unified Malayalam article-summary corpus.

After preprocessing and filtering, the resulting corpus contained:

**9,698 Malayalam article-summary pairs.**

## Dataset Splits

| Split | Samples |
|---|---:|
| Train | 7,758 |
| Validation | 970 |
| Test | 970 |
| Overall | 9,698 |
