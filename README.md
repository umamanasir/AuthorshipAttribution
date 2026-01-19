# Authorship Attribution
This repo contains the model for authorship attribution using machine learning. It identifies the author of a given tweet from a group of Twitter users. 

Phase 1 of the project focused on data preparation and phase 2 focused on modeling & evaluation.

### Phase 1: Data Preparation
1. Scraping and cleaning tweets.
2. Feature extraction using Bag of Words and Laplace smoothing.

### Phase 2: Modeling & Eval
1. Feature engineering using both BoW and BERT-based sentence embeddings.
2. Model training using KNNs, Neural Networks, and Ensemble Methods.
3. Performance evaluation using accuracy, precision, recall, F1-score, and confusion matrices.

## Details: 
Phase 1 involved:
1. Scrapping 1000+ tweets from the a Twitter account. 
2. Data cleaning techniques were applied included using regex to clear out stopwords, lowercasing, Punctuation & URL removal and tokenization.
3. BoW feature vectors & Add-1(Laplace) smoothing was done to avoid zero-frequency issues.

Phase 2 involved: 
1. Tweets were combined from all group members to create BoW & BERT-based features. 
2. KNN-Classifier with 5-fold cross-validation. 
3. Neural Network Classifier using Sciki-Learn's MLPClassifier
4. Ensemble Methods - Bagging, Boosting & Voting ensembles. 


## Results:
| Model       | Features | Accuracy | 
|-------------|----------|----------|
| KNN         | BoW      | 60.7%    |
| KNN         | BERT     | 81.8%    |
| NN          | BoW      | 84%      |
| NN          | BERT     | 81.6%    |
| Ensemble    | BOW      | 85%      |
| Ensemble    | BERT     | 86%      | 

Ensemble methods showed the best results! 



