# Reviews Sentiment Dataset

## 📌 Overview

This dataset is a sentiment analysis dataset designed for multimodal machine learning tasks combining **text, tabular, categorical, and temporal features**. It simulates real-world e-commerce review data inspired by public Amazon Reviews datasets.

It is ideal for:

* NLP + Tabular ML projects
* Sentiment classification
* Feature engineering practice
* Academic assignments and ML projects

---

## 📂 Files Included

* `train.csv` — 20,000 labeled samples
* `test.csv` — 10,000 unlabeled samples
* `sample.csv` — Submission format (`id`, `sentiment`)

---

## 🧾 Dataset Schema

| Column Name         | Type                | Description                                       |
| ------------------- | ------------------- | ------------------------------------------------- |
| `id`                | Integer             | Unique review identifier                          |
| `review_date`       | Date                | Date of the review                                |
| `product_category`  | Categorical         | Product domain (e.g., Electronics, Books, Beauty) |
| `verified_purchase` | Boolean             | Whether the purchase was verified                 |
| `rating`            | Numerical (1–5)     | Star rating given by the user                     |
| `helpful_votes`     | Numerical           | Number of helpful votes                           |
| `total_votes`       | Numerical           | Total votes received                              |
| `review_text`       | Text                | Customer review content                           |
| `sentiment`         | Target (train only) | Sentiment label: positive / neutral / negative    |

---

## 🎯 Target Variable

The target variable is `sentiment`, derived from rating:

* `positive` → Rating ≥ 4
* `neutral` → Rating = 3
* `negative` → Rating ≤ 2

---

## 🚀 Recommended Use Cases

* Sentiment Analysis (Text Classification)
* Hybrid Models (Text + Tabular Features)
* Feature Engineering Practice
* TF-IDF / Embeddings + ML Models
* LightGBM, XGBoost, Logistic Regression

---

## 🧠 Suggested Baseline Workflow

1. Text preprocessing (cleaning, TF-IDF, n-grams)
2. Extract date features (year, month, recency)
3. Encode categorical features (One-Hot / Target Encoding)
4. Train classification models
5. Evaluate using Accuracy / F1-score

---


## 📜 License

This dataset is generated for educational and non-commercial use.
