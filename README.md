# Novel Fusion of Graph Convolution and Language Models for Sentiment and Topic Analysis in Low-Resource Languages


## Abstract

In the nascent field of Natural Language Processing (NLP) for the Filipino language, the scarcity of publicly accessible corpora and labeled datasets presents significant challenges for model training and validation. Concurrently, the potential of graph-based NLP models for analyzing the variable nature of social media text remains underexplored. To address these gaps, our research makes several key contributions. First, we have constructed a substantial dataset, comprising 9,000 manually annotated and 600,000 weakly labeled Filipino tweets related to the 2022 Philippine National Elections, to enhance model training and evaluation. Second, we introduce an innovative model that synergistically combines the strengths of BERT with Graph Convolutional Network (GCN) and enriches training with the inclusion of emojis, hashtags, and user mentions. This model outperforms 16 compared models and achieves an overall F1-score of 0.78 in sentiment classification, indicating that emotional nuances embedded within graph learning coupled with BERT embeddings can yield robust predictions in imbalanced datasets. Finally, we offer a novel topic modeling framework that leverages Bert-LDA alongside the Log-likelihood Ratio to enable the extraction of pivotal information from tweets. This framework successfully discerns key narratives from the 2022 elections within five distinct topic clusters, providing comprehensive insights into the election discourse.


## Model Architecture

<img width="1305" alt="image" src="https://github.com/nlptmu/EmoBERTGCN/assets/95019423/78140249-94b4-49fa-9ab1-2de3d1356e13">


## Model Evaluation Results

<img width="1052" alt="image" src="https://github.com/nlptmu/EmoBERTGCN/assets/95019423/dad64b6d-fb56-40af-9e6e-5b8c3260f60c">


## Tweet Distribution

<img width="318" alt="image" src="https://github.com/nlptmu/EmoBERTGCN/assets/95019423/c74e67f7-6fc5-4512-8208-ea8bdb74913e">


## Topic Word Clouds

<img width="947" alt="image" src="https://github.com/nlptmu/EmoBERTGCN/assets/95019423/12f54c11-f2e6-4b6c-a19d-e25feaa11042">




