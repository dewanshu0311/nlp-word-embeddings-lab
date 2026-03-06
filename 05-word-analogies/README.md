# 👑 Lab 5: Word Analogies

## Objective

Explore the famous **King − Man + Woman = Queen** analogy using vector arithmetic on word embeddings.

## Key Concepts

- Word embeddings encode relationships as vector offsets
- Vector arithmetic: `king - man + woman ≈ queen`
- Analogy tasks as a benchmark for embedding quality
- Limitations of vector analogies (not all relationships are linear)

## Classic Analogies Tested

| Analogy | Expected Result |
|---------|----------------|
| king − man + woman | queen |
| paris − france + japan | tokyo |
| bigger − big + small | smaller |

## Key Finding

> Vector arithmetic works surprisingly well for common relationships (gender, geography, grammar), but breaks down for abstract or cultural associations. This reveals both the power and limitations of embedding geometry.

## How to Run

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/dewanshu0311/nlp-word-embeddings-lab/blob/main/05-word-analogies/lab5_word_analogies.ipynb)

## Technologies

- Gensim (pre-trained Word2Vec / GloVe)
- NumPy
- Python
