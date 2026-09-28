# Multilingual Models

Four multilingual models were selected to examine different model architectures and multilingual/Indic-language capabilities.

## mBART

mBART is a multilingual encoder-decoder Transformer model.

The encoder processes the input article and produces contextual representations. The decoder then generates the Malayalam summary autoregressively based on the encoded representation and previously generated tokens.

## mT5

mT5 is a multilingual text-to-text Transformer based on an encoder-decoder architecture.

The input article is processed by the encoder, while the decoder generates the target Malayalam summary token by token.

## BLOOMZ

BLOOMZ is a multilingual decoder-only language model.

Unlike encoder-decoder models, the input and generated output are handled within a single autoregressive sequence, with the model generating the continuation based on the supplied prompt and article.

## Sarvam

Sarvam is an Indic-centric multilingual model included to examine the performance of an Indian-language-oriented model alongside general multilingual models.

## Model Comparison

| Model | Architecture / Orientation |
|---|---|
| mBART | Encoder-decoder |
| mT5 | Encoder-decoder |
| BLOOMZ | Decoder-only |
| Sarvam | Indic-centric multilingual |
