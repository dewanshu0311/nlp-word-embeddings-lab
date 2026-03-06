# 🧠 NLP Word Embeddings Lab — From Basics to Sentiment Intelligence

A structured, hands-on NLP portfolio covering **word embeddings** from first principles to a production-style **Twitter Sentiment Intelligence System**. Five progressive labs build understanding of embedding concepts, culminating in a capstone project that classifies 1.6M tweets using Gemini embeddings + XGBoost.

---

## 📚 Learning Journey

| # | Lab | Key Concepts | Notebook |
|---|-----|-------------|----------|
| 1 | **Basic Embeddings** | Gemini API, vector dimensions, embedding inspection | [Lab 1](01-basic-embeddings/lab1_gemini_embeddings.ipynb) |
| 2 | **Semantic Similarity** | Cosine similarity, word vs sentence comparison, mini search engine | [Lab 2](02-semantic-similarity/lab2_semantic_similarity.ipynb) |
| 3 | **Contextual Embeddings** | BERT vs ELMo vs Word2Vec, static vs contextual analysis | [Lab 3](03-contextual-embeddings/lab3_contextual_embeddings.ipynb) |
| 4 | **Sentiment Classification** | IMDB dataset, Gemini embeddings → XGBoost classifier | [Lab 4](04-sentiment-classification/lab4_sentiment_classification.ipynb) |
| 5 | **Word Analogies** | King − Man + Woman = Queen, vector arithmetic, limitations | [Lab 5](05-word-analogies/lab5_word_analogies.ipynb) |
| 🏆 | **Twitter Sentiment Project** | 1.6M tweets, full EDA → embeddings → multi-model evaluation → insights | [Final Project](FINAL_TWITTER_SENTIMENT_PROJECT/twitter_sentiment_embeddings_project.ipynb) |

---

## 🏗️ Pipeline Architecture

```
                  ┌──────────────────┐
                  │   Raw Text Data  │
                  │  (Tweets / IMDB) │
                  └────────┬─────────┘
                           │
                           ▼
              ┌────────────────────────┐
              │     Preprocessing      │
              │  Clean → Normalize →   │
              │  Remove noise          │
              └────────────┬───────────┘
                           │
                           ▼
              ┌────────────────────────┐
              │   Gemini Embeddings    │
              │   text-embedding-004   │
              │   768-dim vectors      │
              └────────────┬───────────┘
                           │
              ┌────────────┴───────────┐
              │                        │
              ▼                        ▼
   ┌──────────────────┐   ┌──────────────────┐
   │   Visualization  │   │   ML Classifier  │
   │   PCA / Scatter  │   │   XGBoost / LR   │
   │   Clusters       │   │   SVM / RF       │
   └──────────────────┘   └────────┬─────────┘
                                   │
                                   ▼
                        ┌──────────────────┐
                        │   Evaluation     │
                        │   Accuracy, F1   │
                        │   Confusion Mat  │
                        └──────────────────┘
```

---

## ✨ Features

| Feature | Description |
|---------|-------------|
| **Progressive Labs** | 5 labs that build on each other, from embedding basics to real classification |
| **Gemini Embeddings** | Uses Google's `text-embedding-004` model (768-dim vectors) |
| **Multi-Model Comparison** | XGBoost, Logistic Regression, SVM, Random Forest side-by-side |
| **Rich EDA** | Word clouds, sentiment distributions, text length analysis |
| **PCA Visualization** | 2D scatter plots showing sentiment clusters in embedding space |
| **1.6M Tweet Dataset** | Large-scale Twitter data for the capstone project |
| **Insights & Recommendations** | Business-actionable findings from sentiment analysis |
| **Colab-Ready** | All notebooks run directly in Google Colab with one click |

---

## 📁 Project Structure

```
nlp-word-embeddings-lab/
├── 01-basic-embeddings/
│   ├── README.md
│   └── lab1_gemini_embeddings.ipynb         # Embed text, inspect vectors
├── 02-semantic-similarity/
│   ├── README.md
│   └── lab2_semantic_similarity.ipynb       # Cosine similarity + mini search
├── 03-contextual-embeddings/
│   ├── README.md
│   └── lab3_contextual_embeddings.ipynb     # BERT vs Word2Vec comparison
├── 04-sentiment-classification/
│   ├── README.md
│   └── lab4_sentiment_classification.ipynb  # IMDB → XGBoost classifier
├── 05-word-analogies/
│   ├── README.md
│   └── lab5_word_analogies.ipynb            # Vector arithmetic experiments
├── FINAL_TWITTER_SENTIMENT_PROJECT/
│   ├── README.md
│   └── twitter_sentiment_embeddings_project.ipynb  # ⭐ Capstone
├── docs/
│   └── Insights_and_Recommendations.md      # Key findings & recommendations
├── data/                                     # Dataset directory
├── references/                               # Papers & resources
├── .github/workflows/ci.yaml                # CI pipeline
├── requirements.txt
├── LICENSE
└── README.md                                 # ← You are here
```

---

## 📊 Final Project — Twitter Sentiment Intelligence

The capstone project applies everything learned across the labs to a **real-world Twitter sentiment analysis** task:

### Dataset
- **Sentiment140** — 1.6 million tweets labeled as positive (4) or negative (0)
- Features: tweet text, target sentiment, date, user

### What It Covers
1. **Exploratory Data Analysis** — sentiment distribution, word clouds, text length patterns
2. **Preprocessing** — cleaning tweets, handling mentions, URLs, special characters
3. **Embedding Generation** — batch encoding with Gemini `text-embedding-004`
4. **Multi-Model Training** — XGBoost, Logistic Regression, SVM, Random Forest
5. **Evaluation** — accuracy, F1-score, confusion matrices, classification reports
6. **Custom Predictions** — 5 real-world tweet predictions with confidence scores
7. **Insights & Recommendations** — actionable findings: [Full Report](docs/Insights_and_Recommendations.md)

---

## 🚀 Quick Start

```bash
# Clone the repository
git clone https://github.com/dewanshu0311/nlp-word-embeddings-lab.git
cd nlp-word-embeddings-lab

# Install dependencies
pip install -r requirements.txt

# Open any notebook in Colab or Jupyter
jupyter notebook
```

> **Note:** All notebooks use the Gemini API. You'll need a [Google AI Studio](https://aistudio.google.com/) API key (free tier works).

---

## 🛠️ Technologies

| Category | Technology |
|----------|------------|
| **Embeddings** | Google Gemini (`text-embedding-004`, 768-dim) |
| **ML Models** | XGBoost, Logistic Regression, SVM, Random Forest |
| **NLP** | Gensim (Word2Vec), scikit-learn |
| **Visualization** | matplotlib, seaborn, WordCloud, PCA |
| **Data** | pandas, NumPy |
| **Environment** | Google Colab, Jupyter Notebook |
| **CI** | GitHub Actions |

---

## 💡 Key Insights

Analysis of the Twitter sentiment data reveals:

- **Embedding quality matters** — Gemini embeddings significantly outperform traditional bag-of-words for sentiment classification
- **Simple models work** — even Logistic Regression achieves strong results when features (embeddings) are good
- **Sentiment clusters are separable** — PCA visualization shows clear positive/negative clusters in embedding space
- **Short text is hard** — tweets with sarcasm, slang, or mixed sentiment remain challenging for all models
- **Recommendation:** Combine embedding-based classifiers with rule-based systems for edge cases (sarcasm, negation)

Full report: [docs/Insights_and_Recommendations.md](docs/Insights_and_Recommendations.md)

---

## 📜 License

This project is licensed under the MIT License. Datasets are sourced from Kaggle / Sentiment140 under their respective licenses.
