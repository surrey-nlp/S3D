<p align="center"><img src="./imgs/icon.svg"></p>

# S3D: A Weakly Supervised Sarcasm Dataset

This is the repository for our 'Utilizing Weak Supervision to Create S3D: A Sarcasm Annotated Dataset' paper submitted to the EMNLP NLP+CSS 2022 workshop. This repository includes our SAD dataset along with version 1 and 2 of our S3D dataset. Both of these twitter datasets can be used for the purpose of training sarcasm detection models.

### Datasets

SAD - We provide the Tweet IDs and the given sarcasm labels of 2340 manually annotated tweets which were collected observing the #sarcasm hashtag.

S3D-v1 - We provide the Tweet IDs of 100,000 tweets along with their respective labels which were predicted by a fine-tuned BERTweet model which was trained on our 'Combined dataset', a corpus of over a million tweets and reddit comments labelled for sarcasm in previous works.

S3D-v2 - We provide the Tweet IDs of 100,000 tweets along with their respective labels which were predicted by an ensemble of our 'best' three fine-tuned sarcasm detection models.

### Experiments

We provide a notebook to show the labelling process of our S3D-v1 dataset. We aim to have a notebook ready to demonstrate the majority voting annotations very soon.

### Models

| **Models** | **Fine-tuned Models** | **Description**                                   |
|------------|-----------------------|---------------------------------------------------|
| [BERTweet](https://huggingface.co/docs/transformers/model_doc/bertweet)   | Coming soon                   | BERTweet model fine-tuned on our combined dataset |
| [BERTweet](https://huggingface.co/docs/transformers/model_doc/bertweet)  |  [BERTweet-base-finetuned-SARC-DS](https://huggingface.co/surrey-nlp/bertweet-base-finetuned-SARC-DS)                    | BERTweet model fine-tuned on the SARC dataset                   |
| [RoBERTa<sub>large</sub>](https://huggingface.co/roberta-large)  | Coming soon                     | RoBERTa<sub>large</sub> model fine-tuned on our combined dataset                   |
## Maintainer(s)
[Jordan Painter](https://github.com/jordanpainter) <br/>
[Diptesh Kanojia](https://dipteshkanojia.github.io)
