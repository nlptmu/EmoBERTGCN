# Novel Fusion of Graph Convolution and Language Models for Sentiment and Topic Analysis in Low-Resource Languages


## Abstract

In the nascent field of Natural Language Processing (NLP) for the Filipino language, the scarcity of publicly accessible corpora and labeled datasets presents significant challenges for model training and validation. Concurrently, the potential of graph-based NLP models for analyzing the variable nature of social media text remains underexplored. To address these gaps, our research makes several key contributions. First, we have constructed a substantial dataset, comprising 9,000 manually annotated and 600,000 weakly labeled Filipino tweets related to the 2022 Philippine National Elections, to enhance model training and evaluation. Second, we introduce an innovative model that synergistically combines the strengths of BERT with Graph Convolutional Network (GCN) and enriches training with the inclusion of emojis, hashtags, and user mentions. This model outperforms 16 compared models and achieves an overall F1-score of 0.78 in sentiment classification, indicating that emotional nuances embedded within graph learning coupled with BERT embeddings can yield robust predictions in imbalanced datasets. Finally, we offer a novel topic modeling framework that leverages Bert-LDA alongside the Log-likelihood Ratio to enable the extraction of pivotal information from tweets. This framework successfully discerns key narratives from the 2022 elections within five distinct topic clusters, providing comprehensive insights into the election discourse.


## Model Architecture

<img width="1305" alt="image" src="https://github.com/nlptmu/EmoBERTGCN/assets/95019423/78140249-94b4-49fa-9ab1-2de3d1356e13">


## Model Evaluation Results

Model	Precision	Recall	F1-score
Naïve Bayes	0.5866	0.3453	0.4594
KNN	0.6752	0.5671	0.6747
Decision Tree	0.5113	0.5018	0.6267
Logistic Regression	0.8017	0.5555	0.7250
Support Vector Machine	0.8587	0.5355	0.6986
Passive Aggressive	0.6519	0.5788	0.7290
Ridge Classifier	0.7783	0.5740	0.7298
Light GBM	0.7311	0.5647	0.7178
Adaboost	0.6234	0.5140	0.6742
Random Forest	0.9308	0.4680	0.5829
XG Boost	0.7466	0.5415	0.6927
Catboost	0.7645	0.5437	0.7010
FFNN	0.8851	0.5079	0.6558
BiLSTM	0.6590	0.5636	0.6935
TextCNN	0.7687	0.5697	0.7008
BertGCN 	0.8320	0.6146	0.7624
EmoBERTGCN	0.7453	0.6787	0.7803
![image](https://github.com/nlptmu/EmoBERTGCN/assets/95019423/4ee7c1d4-41c6-446b-9b6b-a4262f8fd7bc)

