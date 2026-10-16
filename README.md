# kaggle_first_nlp_model
First NLP Kaggle competition, building simple baseline models: Logistic Regression, Naive Bayes, LSTMs, GRUs, and eventually fine-tuning a basic transformer model. 

## Natural Language Processing with Disaster Tweets

This repository contains my solution and notebook for the Kaggle competition: [Natural Language Processing with Disaster Tweets](https://www.kaggle.com/c/nlp-getting-started). 

## Project Goals

This was my first Kaggle competition for NLP. The primary aim here was to learn and become more comfortable with:

Text cleaning and preprocessing (handling hashtags, URLs, etc.)

Classic feature extraction techniques like Bag-of-Words and TF-IDF

Building simple baseline machine learning models (Logistic Regression, Naive Bayes)

Exploring deep learning approaches (LSTMs, GRUs, and fine-tuning a basic Transformer like DistilBERT)

The Task: Predict whether a given tweet is about a real disaster or not (binary text classification).

Data Exploration & Preprocessing

EDA: Analyzed word frequencies, bigrams, and tweet metadata. Discovered that URLs are significantly more common in real disaster tweets (often linking to news), while non-disaster tweets feature more casual language.

Cleaning: Standardized text by lowercasing, removing HTML entities, and replacing URLs and user mentions with special <URL> and <USER> tokens to preserve their signal without adding noise.

## Models Built

I experimented with four different models, ranging from simple baselines to more complex architectures:

Logistic Regression: Combined with a TfidfVectorizer.

Naive Bayes: MultinomialNB using word frequencies.

LSTM: A deep learning model built with TensorFlow/Keras, utilizing an Embedding layer and a Bidirectional LSTM.

DistilBERT: A modern, transformer-based model fine-tuned using the keras_nlp library.

## Results & Submission

Based on validation metrics (accuracy, F1-score, and AUC), the Logistic Regression model achieved the highest F1-score (0.755) and was selected as the best performer for the final submission.

Best Kaggle Score: 0.78853 (V4)

Note: I think that score is about average. Regardless, this served as an excellent introductory project for NLP concepts and model building.
