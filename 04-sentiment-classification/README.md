# 🎯 Lab 4: Sentiment Classification with Embeddings

## Objective

Use text embeddings as input features to train a classical machine learning model for **sentiment classification** on the IMDB movie reviews dataset.

## Key Concepts

- Embeddings as ML features — converting text to fixed-length vectors
- IMDB movie reviews dataset (50,000 reviews, binary sentiment)
- XGBoost classifier trained on Gemini embedding vectors
- Model evaluation using accuracy, precision, recall, F1-score
- Custom prediction on user-input reviews

## Steps Performed

1. Load and preprocess the IMDB dataset
2. Convert text reviews into embeddings using Gemini API
3. Split data into training and testing sets
4. Train an XGBoost classifier on embedding vectors
5. Evaluate the model using accuracy and classification report
6. Test the model on custom user inputs

## Key Finding

> Even simple classifiers (XGBoost) perform extremely well when powered by high-quality Gemini embeddings. This approach is commonly used in production NLP systems where speed and interpretability matter.

## How to Run

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/dewanshu0311/nlp-word-embeddings-lab/blob/main/04-sentiment-classification/lab4_sentiment_classification.ipynb)

## Technologies

- Google Gemini API (`text-embedding-004`)
- XGBoost
- scikit-learn
- pandas, NumPy
