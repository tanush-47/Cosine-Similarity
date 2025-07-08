# Cosine Similarity

This Python project demonstrates how to compute the **cosine similarity** between two text documents using **TF-IDF (Term Frequency–Inverse Document Frequency)** vectorization. Cosine similarity is a measure used to determine how similar two texts are, regardless of their size.

## 🔍 What is Cosine Similarity?

Cosine similarity calculates the cosine of the angle between two non-zero vectors in an inner product space. It is widely used in text analysis and NLP for comparing document similarity.

The similarity score ranges from:
- `1` → documents are **exactly similar**
- `0` → documents are **completely dissimilar**

## 📂 Project Structure

Cosine-Similarity/

├── cosine_similarity.py # Main script for calculating cosine similarity

├── requirements.txt # Python dependencies

└── README.md # Project documentation


## 🧠 How It Works

1. Takes two input text documents (strings).
2. Uses `TfidfVectorizer` from `sklearn` to convert text into vector form.
3. Calculates cosine similarity using `cosine_similarity()` function.

## 🚀 Getting Started

### ✅ Prerequisites

- Python 3.6+
- pip

### 📦 Install Dependencies

```bash
pip install -r requirements.txt
