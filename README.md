# EmoBERTGCN-sentiment-analysis

## Abstract

Natural language processing (NLP) research for the Filipino language is relatively new and emerging, as compared to high resource languages like English. There are only a very limited amount of publicly available corpora and labelled datasets suitable for model training and evaluation. Meanwhile, there has been a surge of interest on investigating the effectiveness of graph-based NLP models, but their performances on highly variable social media texts is not sufficiently explored. Therefore, this work attempts to alleviate these issues by making the following contributions. First, we create a large-scale dataset with nine thousand manually annotated and 600 thousand weakly labelled Tweets in Filipino concerning the 2022 Philippine National Elections. Second, we propose a new model that integrates BERT and Graph Convolutional Network (GCN) modules, and incorporates emojis, hashtags and user mentions in the model training process with the manually annotated dataset. Besting the baseline models, it achieves 0.679 macro recall score and 0.78 macro F1 score for binary sentiment classification. This suggests that emotion-infused graph learning paired with BERT embeddings can provide robust predictions even in imbalanced datasets. The proposed model is further used to predict the labels of the weakly labelled dataset. Third, we present a topic modelling framework employing BERT-LDA technique and Log-likelihood Ratio keyword extraction to find crucial information contained within the Tweets. In particular, numerous events regarding the 2022 elections can be thoroughly explored within the five topic clusters produced by our framework. It is verified that they are aligned with the official reports of reputable news agencies. 

## Model Architecture

![Capture-2023-08-21-120130](https://github.com/nlptmu/EmoBERTGCN-sentiment-analysis/assets/95019423/a97c4d59-1451-4319-b505-ddacbb13f371)

## Model Evaluation Results

| Model | Recall | F^PN^~1 |
| ----- | -------| -------- |
| Support Vector Machine | 0.5355 | 0.6986 |

## Topic Modelling Process

![Capture-2023-08-21-120154](https://github.com/nlptmu/EmoBERTGCN-sentiment-analysis/assets/95019423/0b5c60c2-afcb-4054-b24b-cc524750ef02)

