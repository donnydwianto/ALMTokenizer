# ALMTokenizer


## Abstract

Recent advancements in audio language models have underscored the pivotal role of audio tokenization, which converts audio signals into discrete tokens, thereby facilitating the application of language model architectures to the audio domain. In this study, we introduce ALMTokenizer, a novel low-bitrate and semantically rich audio codec tokenizer for audio language models. Prior methods, such as Encodec, typically encode individual audio frames into discrete tokens without considering the use of context information across frames. Unlike these methods, we introduce a novel query-based compression strategy to capture holistic information with a set of learnable query tokens by explicitly modeling the context information across frames. This design not only enables the codec model to capture more semantic information but also encodes the audio signal with fewer token sequences. Additionally, to enhance the semantic information in audio codec models, we introduce the following: (1) A masked autoencoder (MAE) loss, (2) Vector quantization based on semantic priors, and (3) An autoregressive (AR) prediction loss. As a result, ALMTokenizer achieves competitive reconstruction performance relative to state-of-the-art approaches while operating at a lower bitrate. Within the same audio language model framework, ALMTokenizer outperforms previous tokenizers in audio understanding and generation tasks

