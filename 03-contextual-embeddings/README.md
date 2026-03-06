# 🧠 Lab 3: Contextual Embeddings

## Objective

Compare **contextual embeddings** (BERT, ELMo) with **static embeddings** (Word2Vec) to understand how context changes meaning representation.

## Key Concepts

- Static vs contextual embeddings: why context matters
- Word2Vec — one fixed vector per word regardless of context
- BERT / ELMo — different vectors for the same word in different sentences
- Example: "bank" (river bank) vs "bank" (financial bank) → same vector in Word2Vec, different vectors in BERT

## Key Finding

> Contextual models produce different embeddings for the same word depending on surrounding context, which is critical for tasks like sentiment analysis where "not bad" should not mean the same as "bad."

## How to Run

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/dewanshu0311/nlp-word-embeddings-lab/blob/main/03-contextual-embeddings/lab3_contextual_embeddings.ipynb)

## Technologies

- BERT (Hugging Face Transformers)
- Gensim (Word2Vec)
- NumPy, matplotlib
