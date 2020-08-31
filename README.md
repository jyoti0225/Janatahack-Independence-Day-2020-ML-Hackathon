# Janatahack-Independence-Day-2020-ML-Hackathon
This hackathon was organised by Analytics Vidya to showcase machine learning skills by sharing approaches and more important to learn how to apply machine learning and predictive analytics to new domains. In this hackathon, we have to perform Topic Modeling for Research Articles.It is a multi-label classification problem.<br>
In this repository, I used machine learning and deep learning models along with NLP to solve this problem.

## Problem Statement - 
Researchers have access to large online archives of scientific articles. As a consequence, finding relevant articles has become more difficult. Tagging or topic modelling provides a way to give token of identification to research articles which facilitates recommendation and search process.

Given the abstract and title for a set of research articles, predict the topics for each article included in the test set. Note that a research article can possibly have more than 1 topic. The research article abstracts and titles are sourced from the following 6 topics: 

1. Computer Science
2. Physics
3. Mathematics
4. Statistics
5. Quantitative Biology
6. Quantitative Finance

## Scores
Public Leaderboard - 23 rank </br>
Private Learderboard - 15 rank

## Approaches
For preprocessing, first of all I cleaned the data using NLP (remove stopwords,noise,lemmatization).Then to covert the text into vectors, I used TFIDF(term frequency–inverse document frequency) vectorizer. Now comes the model building part. For that, I have implemented 2 approches - 
#### 1. Machine Learning Models
Since, it is a multi-label classification problem, therefore tried different models like Logistic Regression, SVM, Naive Bayes, etc along with OneVsRestClassifier to predict the target classes.
#### 2. Deep Neural Network
This gives me better accuracy then the previous approach. The preprocessing steps remains the same as discussed above. After conveting the text into vectors using TFIDF, the vectors are passed to the Artificial Neural Network which consists of Dense layers and Dropout was also applied to avoid overfitting. This prediction gives me 23 rank on Public Leaderboard and 15 rank on Private Learderboard.
