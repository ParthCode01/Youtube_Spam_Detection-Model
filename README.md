# 📺 YouTube Spam Comment Detection

This project builds a machine learning model to detect spam comments on YouTube videos using natural language processing techniques.

## 💡 Problem Statement
YouTube videos often receive a large number of spam comments. This project trains a classifier to automatically identify whether a comment is **spam** or **not spam**.

## 📁 Dataset
We used the [YouTube Spam Collection Dataset](https://archive.ics.uci.edu/ml/datasets/YouTube+Spam+Collection), specifically:
- `Youtube04-Eminem.csv`

Each entry contains:
- **CONTENT**: The actual comment text
- **CLASS**: `1` for spam, `0` for not spam

## 🧠 Model Pipeline

1. **Data Preprocessing**
   - Text cleaning
   - Removing duplicates and nulls

2. **Feature Extraction**
   - `TfidfVectorizer` is used to convert text into numerical features

3. **Model Training**
   - Logistic Regression (can be replaced with other models)

4. **Prediction**
   - You can enter a custom comment and the model will classify it as **spam** or **not spam**

## 🚀 Run the Notebook

You can try the notebook on Google Colab:

[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/your-username/your-repo-name/blob/main/your-notebook.ipynb)

## 🔍 Example

```
sample = ["Subscribe to my channel for free cash"]
sample_tf = vectorizer.transform(sample)
model.predict(sample_tf)
# Output: [1] → Spam
