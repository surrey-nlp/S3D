<p align="center"><img src="./imgs/icon.svg" alt="logo" width="270" height="200">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<img src="imgs/aisurrey.svg" alt="Surrey Institute for People-centred AI" width="270"/></p>


# S3D: A Weakly Supervised Sarcasm Dataset

[![GitHub issues](https://img.shields.io/github/issues/surrey-nlp/S3D?style=flat-square)](https://github.com/surrey-nlp/S3D/issues)
[![GitHub stars](https://img.shields.io/github/stars/surrey-nlp/S3D?style=flat-square)](https://github.com/surrey-nlp/S3D/stargazers)
[![GitHub forks](https://img.shields.io/github/forks/surrey-nlp/S3D?style=flat-square)](https://github.com/surrey-nlp/S3D/network)
[![License: CC BY-SA 4.0](https://img.shields.io/badge/License-CC_BY--SA_4.0-lightgrey.svg)](https://creativecommons.org/licenses/by-sa/4.0/)
[![Twitter Follow](https://img.shields.io/twitter/follow/PeopleCentredAI?color=1DA1F2&logo=twitter&style=flat-square)](https://twitter.com/PeopleCentredAI)

This is the repository for our 'Utilizing Weak Supervision to Create S3D: A Sarcasm Annotated Dataset' paper submitted to the EMNLP NLP+CSS 2022 workshop. This repository includes our SAD dataset along with version 1 and 2 of our S3D dataset. Both of these twitter datasets can be used for the purpose of training sarcasm detection models.

### Datasets

SAD - We provide the Tweet IDs and the given sarcasm labels of 2340 manually annotated tweets which were collected observing the #sarcasm hashtag. [Available on HuggingFace](https://huggingface.co/datasets/surrey-nlp/SAD)

S3D-v1 - We provide the Tweet IDs of 100,000 tweets along with their respective labels which were predicted by a fine-tuned BERTweet model which was trained on our 'Combined dataset', a corpus of over a million tweets and reddit comments labelled for sarcasm in previous works. [Available on HuggingFace](https://huggingface.co/datasets/surrey-nlp/S3D-v1)

S3D-v2 - We provide the Tweet IDs of 100,000 tweets along with their respective labels which were predicted by an ensemble of our 'best' three fine-tuned sarcasm detection models. [Available on HuggingFace](https://huggingface.co/datasets/surrey-nlp/S3D-v2)

### Experiments

We provide a notebook to show the labelling process of our datasets. You can reproduce the experiments to create S3D-v1 and S3D-v2 via our Python [notebooks](https://github.com/surrey-nlp/S3D/blob/main/nbs/) which uses HuggingFace to load the relevant models to label the dataset.

### Models

| **Models** | **Fine-tuned Models** | **Description**                                   |
|------------|-----------------------|---------------------------------------------------|
| [BERTweet](https://huggingface.co/docs/transformers/model_doc/bertweet)   |  [BERTweet-base-finetuned-SARC-combined-DS](https://huggingface.co/surrey-nlp/bertweet-base-finetuned-SARC-combined-DS)                  | BERTweet model fine-tuned on our combined dataset |
| [BERTweet](https://huggingface.co/docs/transformers/model_doc/bertweet)  |  [BERTweet-base-finetuned-SARC-DS](https://huggingface.co/surrey-nlp/bertweet-base-finetuned-SARC-DS)                    | BERTweet model fine-tuned on the SARC dataset                   |
| [RoBERTa<sub>large</sub>](https://huggingface.co/roberta-large)  | [roberta-large-finetuned-SARC-combined-DS](https://huggingface.co/surrey-nlp/roberta-large-finetuned-SARC-combined-DS)                     | RoBERTa<sub>large</sub> model fine-tuned on our combined dataset                   |
## Maintainer(s)
[Jordan Painter](https://github.com/jordanpainter) <br/>
[Diptesh Kanojia](https://dipteshkanojia.github.io)
