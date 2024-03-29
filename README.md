# Novel Fusion of Graph Convolution and Language Models for Sentiment and Topic Analysis in Low-Resource Languages


## Abstract

In the nascent field of Natural Language Processing (NLP) for the Filipino language, the scarcity of publicly accessible corpora and labeled datasets presents significant challenges for model training and validation. Concurrently, the potential of graph-based NLP models for analyzing the variable nature of social media text remains underexplored. Addressing these gaps, our research makes several key contributions. Firstly, we have constructed a substantial dataset, comprising 9,000 manually annotated and 600,000 weakly labeled Filipino tweets related to the 2022 Philippine National Elections, to enhance model training and evaluation. Secondly, we introduce an innovative model that synergistically combines the strengths of BERT with Graph Convolutional Network (GCN) frameworks and enriches training with the inclusion of emojis, hashtags, and user mentions. This model outperforms 16 compared models, achieving an overall macro-recall score of 0.6473 in sentiment classification, indicating that emotional nuances embedded within graph learning, when coupled with BERT embeddings, can yield robust predictions in datasets characterized by imbalance. Finally, we offer a novel topic modeling framework that leverages Bert-LDA alongside the Log-likelihood Ratio, enabling the extraction of pivotal information from the tweets. This framework successfully discerns key narratives from the 2022 elections within five distinct topic clusters, providing comprehensive insights into the election discourse.


## Model Architecture

<img width="1244" alt="image" src="https://github.com/nlptmu/EmoBERTGCN/assets/95019423/3a547105-93e1-4ff2-8912-07d6d94d8c03">


## Model Evaluation Results

| Model                | Precision             | Recall                | F1-score             |
|----------------------|-----------------------|-----------------------|----------------------|
| Naïve Bayes          | 0.5798 ± 0.0246       | 0.3439 ± 0.0030       | 0.3081 ± 0.0075      |
| KNN                  | 0.6802 ± 0.0290       | 0.5595 ± 0.0230       | 0.5974 ± 0.0263      |
| Decision Tree        | 0.5494 ± 0.0143       | 0.5213 ± 0.0118       | 0.5246 ± 0.0162      |
| Logistic Regression  | 0.8362 ± 0.0244       | 0.5681 ± 0.0215       | 0.6320 ± 0.0249      |
| Support Vector Machine | 0.8556 ± 0.0361     | 0.5448 ± 0.0254       | 0.6115 ± 0.0311      |
| Passive Aggressive   | 0.6770 ± 0.0274       | 0.6143 ± 0.0256       | 0.6388 ± 0.0272      |
| Ridge Classifier     | 0.8050 ± 0.0233       | 0.5934 ± 0.0181       | 0.6532 ± 0.0218      |
| Light GBM            | 0.7611 ± 0.0315       | 0.5896 ± 0.0236       | 0.6420 ± 0.0264      |
| Adaboost             | 0.6534 ± 0.0221       | 0.5222 ± 0.0252       | 0.5600 ± 0.0276      |
| Random Forest        | 0.8774 ± 0.0376       | 0.4701 ± 0.0198       | 0.5100 ± 0.0259      |
| XG Boost             | 0.7803 ± 0.0242       | 0.5607 ± 0.0197       | 0.6184 ± 0.0227      |
| Catboost             | 0.8059 ± 0.0387       | 0.5483 ± 0.0243       | 0.6080 ± 0.0302      |
| FFNN                 | 0.8349 ± 0.0298       | 0.5162 ± 0.0293       | 0.5761 ± 0.0364      |
| BiLSTM               | 0.6799 ± 0.0262       | 0.6076 ± 0.0195       | 0.6353 ± 0.0208      |
| TextCNN              | 0.6829 ± 0.0521       | 0.5743 ± 0.0267       | 0.6048 ± 0.0277      |
| TextGCN              | 0.4789 ± 0.1620       | 0.5081 ± 0.1224       | 0.4833 ± 0.1338      |
| BertGCN              | 0.7682 ± 0.0532       | 0.6128 ± 0.0355       | 0.6622 ± 0.0342      |
| EmoBERTGCN           | 0.7701 ± 0.0691       | 0.6473 ± 0.0370       | 0.6872 ± 0.0313      |



## Tweet Distribution

<img width="907" alt="image" src="https://github.com/nlptmu/EmoBERTGCN/assets/95019423/4d2fa510-bee7-4e85-8166-1a6ee65de75b">



## Topic Word Clouds

<img width="947" alt="image" src="https://github.com/nlptmu/EmoBERTGCN/assets/95019423/12f54c11-f2e6-4b6c-a19d-e25feaa11042">




