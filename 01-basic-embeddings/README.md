# 🔤 Lab 1: Basic Semantic Visualization

## Objective

Learn how word embeddings work by generating them with the **Google Gemini API** and inspecting their properties.

## Key Concepts

- Generate embeddings using `text-embedding-004` (768 dimensions)
- Embed single and multiple texts
- Inspect vector dimensions and values
- Perform a basic semantic check (cat vs kitten similarity)

## Key Finding

> Basic embeddings don't always preserve dictionary relationships — "cat" and "kitten" can appear far apart in embedding space. This motivates Lab 2's deeper exploration of semantic similarity.

## How to Run

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/dewanshu0311/nlp-word-embeddings-lab/blob/main/01-basic-embeddings/lab1_gemini_embeddings.ipynb)

## Technologies

- Google Gemini API (`text-embedding-004`)
- NumPy
- Python
