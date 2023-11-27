# EmoBertGCN

## Abstract

Natural language processing (NLP) research for the Filipino language is relatively new and emerging, as compared to high resource languages like English. There are only a very limited amount of publicly available corpora and labelled datasets suitable for model training and evaluation. Meanwhile, there has been a surge of interest on investigating the effectiveness of graph-based NLP models, but their performances on highly variable social media texts is not sufficiently explored. Therefore, this work attempts to alleviate these issues by making the following contributions. First, we create a large-scale dataset with nine thousand manually annotated and 600 thousand weakly labelled Tweets in Filipino concerning the 2022 Philippine National Elections. Second, we propose a new model that integrates BERT and Graph Convolutional Network (GCN) modules, and incorporates emojis, hashtags and user mentions in the model training process with the manually annotated dataset. Besting the baseline models, it achieves 0.679 macro recall score and 0.78 macro F1 score for binary sentiment classification. This suggests that emotion-infused graph learning paired with BERT embeddings can provide robust predictions even in imbalanced datasets. The proposed model is further used to predict the labels of the weakly labelled dataset. Third, we present a topic modelling framework employing BERT-LDA technique and Log-likelihood Ratio keyword extraction to find crucial information contained within the Tweets. In particular, numerous events regarding the 2022 elections can be thoroughly explored within the five topic clusters produced by our framework. It is verified that they are aligned with the official reports of reputable news agencies. 

## Model Architecture

<img width="1305" alt="image" src="https://github.com/nlptmu/EmoBERTGCN/assets/95019423/78140249-94b4-49fa-9ab1-2de3d1356e13">


## Model Evaluation Results

| Model | Recall | F<sub>1</sub><sup>PN</sup> |
| ----- | -------| -------- |
| Support Vector Machine | 0.5355 | 0.6986 |
| Naïve Bayes | 0.3453 | 0.4594 |
| KNN | 0.5671 | 0.6747 |
| Decision Tree | 0.5018 | 0.6267 |
| Logistic Regression | 0.5555 | 0.7250 |
| Passive Aggressive | 0.5788 | 0.7298 |
| Ridge Classifier | 0.5740 | 0.7298 |
| Light GBM | 0.5647 | 0.7178 |
| Adaboost | 0.5140 | 0.6742 |
| Random Forest | 0.4680 | 0.5829 |
| Gradient Boosting | 0.5337 | 0.6568 |
| XG Boost | 0.5415 | 0.6927 |
| Catboost | 0.5437 | 0.7010 |
| Feed-Forward Neural Network | 0.5079 | 0.6558 |
| BiLSTM | 0.5636 | 0.6935 |
| TextCNN | 0.5697 | 0.7008 |
| TextGCN | 0.3333 | 0.4302 | 
| BERTGCN | 0.6146 | 0.7624 |
| EmoBertGCN | **0.6787** | **0.7803** |

