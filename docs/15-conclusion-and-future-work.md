# Conclusion and Future Work

## Conclusion

The study presents a comparative framework for Malayalam-to-Malayalam abstractive summarization using mBART, mT5, BLOOMZ, and Sarvam across zero-shot, few-shot, and supervised fine-tuning configurations.

The results indicate that supervised fine-tuning provides stronger task-specific summarization performance than prompt-based inference. Fine-tuned mT5 achieved the strongest overall lexical-generation performance and obtained 84.46% faithfulness with 18.06% hallucination.

The intrinsic NLI evaluation further demonstrates the importance of examining factual consistency in addition to conventional summarization metrics.

Zero-shot and few-shot configurations showed limited lexical overlap and comparatively weaker task adaptation. The relatively higher BERTScore values observed across several configurations indicate that contextual semantic similarity can remain high even when exact lexical overlap is limited.

This highlights the importance of considering contextual meaning rather than relying exclusively on direct lexical matching for Malayalam abstractive summarization.

## Future Work

Future work can investigate larger and more Malayalam-specialized multilingual models.

The dataset and evaluation can be expanded using additional Malayalam summarization resources and complementary factual-consistency evaluation approaches.

Further research can investigate improved multilingual and Indic-centric adaptation strategies for Malayalam summarization.
