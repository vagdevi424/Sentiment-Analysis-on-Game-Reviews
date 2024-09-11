# Sentiment-Analysis-on-Game-Reviews

Problem Statement:
GameSphere, a digital distribution platform for video games, collects user reviews that are vital for developers and potential buyers. The goal of this project is to build a model that can automatically analyze the sentiment of these reviews and classify them as positive or negative. Additionally, the model predicts the probability that a review expresses positive sentiment.

Key Steps in the Project:
Data Preparation:

The dataset contains 17,319 game reviews, each with attributes such as game title, developer, publisher, tags, overview, user review text, and the sentiment (positive or negative).
Preprocessing of the textual data was done using techniques like lowercasing, removing punctuation, stopwords, URLs, and HTML tags. Lemmatization was applied to normalize the text.
Feature Engineering:

TF-IDF Vectorization was used to convert the review text into numerical features, and the categorical features were processed using one-hot encoding.
Tags associated with each game were binarized to create additional features, and numerical columns (e.g., release year) were standardized.
Modeling:

Three classifiers were trained: Logistic Regression, Random Forest, and K-Nearest Neighbors (KNN). GridSearchCV was used to optimize hyperparameters.
Each model's performance was evaluated using 5-fold cross-validation, and metrics such as accuracy, precision, recall, F1-score, and ROC-AUC were reported.
Evaluation:

Logistic Regression showed the best performance with an ROC-AUC score of 0.94 and an accuracy of 87%.
The model was then used to predict the sentiment probabilities on the test dataset provided, and the results were submitted for external evaluation.
This approach not only provides insights into the sentiment of reviews but also helps GameSphere understand the popularity and reception of various games among users.

