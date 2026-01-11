# AI Echo – Sentiment Analysis of User Reviews

## 📌 Project Overview
AI Echo is a Natural Language Processing (NLP) project that analyzes user reviews
of a ChatGPT application and classifies them into **Positive, Neutral, or Negative**
sentiments. The project aims to extract actionable insights to improve customer
experience and product quality.

---

## 🎯 Objectives
- Perform sentiment analysis on user reviews
- Compare traditional ML models with Transformer-based models
- Visualize sentiment trends using an interactive Streamlit dashboard
- Answer key business questions based on sentiment insights

---

## 🗂 Dataset
- **Source**: ChatGPT-style user reviews
- **Features**:
  - review
  - rating (1–5)
  - date
  - location
  - platform (Web/Mobile)
  - version
  - verified_purchase

Sentiment labels are derived from ratings:
- 4–5 → Positive
- 3 → Neutral
- 1–2 → Negative

---

## 🔧 Technologies Used
- **Language**: Python
- **Libraries**:
  - Pandas, NumPy
  - NLTK
  - Scikit-learn
  - Transformers (BERT)
  - Matplotlib, Seaborn, WordCloud
  - Streamlit
- **Platform**: Google Colab

---

## 🧪 Methodology

### 1. Data Preprocessing
- Lowercasing
- Removal of punctuation and special characters
- Stopword removal
- Lemmatization

### 2. Exploratory Data Analysis (EDA)
- Sentiment distribution
- Keyword analysis using word clouds
- Trends over time
- Platform, location, and version-based analysis

### 3. Sentiment Classification Models

#### Traditional ML
- TF-IDF Vectorization
- Logistic Regression (with class weighting)

#### Transformer-Based Model
- Pretrained BERT embeddings
- Logistic Regression classifier on embeddings
- Used for contextual comparison

> Note: High accuracy is observed due to strong alignment between review text
and rating-based sentiment labels in the dataset.

---

## 📊 Model Evaluation
- Accuracy
- Precision, Recall, F1-score
- Confusion Matrix

---

## 🌐 Streamlit Dashboard
An interactive dashboard was built using Streamlit to answer key questions:
- Overall sentiment distribution
- Sentiment vs rating mismatch
- Keyword analysis per sentiment
- Sentiment trends over time
- Verified vs non-verified users
- Platform, location, and version analysis
- Negative feedback themes

---

## 🚀 How to Run the Project

### 1. Install Dependencies
```bash
pip install -r requirements.txt
