# 🏆 Twitter Sentiment Intelligence System using Embeddings

## Overview

The capstone project of the NLP Word Embeddings Lab — a full-scale **sentiment analysis pipeline** applied to **1.6 million tweets** from the Sentiment140 dataset.

This project demonstrates the end-to-end process of building a production-style sentiment classifier using Google Gemini embeddings and multiple machine learning models.

---

## Pipeline

```
  Raw Tweets (1.6M)
        │
        ▼
  Preprocessing (clean, normalize)
        │
        ▼
  Gemini Embeddings (768-dim vectors)
        │
        ├──→ PCA Visualization (sentiment clusters)
        │
        ▼
  Model Training
  ├── XGBoost
  ├── Logistic Regression
  ├── SVM
  └── Random Forest
        │
        ▼
  Evaluation (accuracy, F1, confusion matrix)
        │
        ▼
  Custom Predictions (5 real-world tweets)
        │
        ▼
  Insights & Recommendations
```

---

## What's Inside

| Section | Description |
|---------|-------------|
| **EDA** | Sentiment distribution, word clouds, text length analysis |
| **Preprocessing** | Tweet cleaning — mentions, URLs, special characters |
| **Embeddings** | Batch encoding with Gemini `text-embedding-004` |
| **Training** | 4 classifiers compared side-by-side |
| **Evaluation** | Accuracy, F1-score, confusion matrices |
| **Predictions** | 5 custom tweet predictions with confidence |
| **Insights** | [Full Report](../docs/Insights_and_Recommendations.md) |

---

## Dataset

**Sentiment140** — 1.6 million tweets labeled as:
- `0` → Negative sentiment
- `4` → Positive sentiment

**Source:** [Kaggle — Sentiment140 Dataset](https://www.kaggle.com/datasets/kazanova/sentiment140)

---

## How to Run

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/dewanshu0311/nlp-word-embeddings-lab/blob/main/FINAL_TWITTER_SENTIMENT_PROJECT/twitter_sentiment_embeddings_project.ipynb)

> **Requires:** Google Gemini API key (free tier from [AI Studio](https://aistudio.google.com/))

---

## Technologies

- Google Gemini API (`text-embedding-004`)
- XGBoost, Logistic Regression, SVM, Random Forest
- scikit-learn, pandas, NumPy
- matplotlib, seaborn, WordCloud
