
---

# The Social Dilemma: Twitter Sentiment Analysis 🐦🤖

This repository contains a comprehensive Natural Language Processing (NLP) project that analyzes public sentiment following the release of the Netflix documentary, **"The Social Dilemma."** The project covers the entire data science lifecycle—from raw data cleaning and exploratory analysis to building machine learning classifiers.

## 📋 Project Overview

The documentary explores how social media algorithms influence human behavior. This project aims to quantify public reaction by analyzing over 20,000 tweets associated with the `#TheSocialDilemma` hashtag.

**The main objectives are:**

* **Data Wrangling:** Cleaning structured and unstructured Twitter data.
* **Text Preprocessing:** Preparing raw text for machine learning.
* **Sentiment Classification:** Building models to categorize tweets as **Positive**, **Negative**, or **Neutral**.
* **Insight Generation:** Visualizing key themes and model performance.

---

## 📊 Dataset Insights

The dataset (`TheSocialDilemma.csv`) consists of approximately **20,068 tweets**.

### Data Cleaning & Analysis

* **Missing Values:** Handled missing data in `user_location` and `hashtags`.
* **Language Filtering:** Removed non-English tweets (maintaining 20,005 valid entries) to ensure the accuracy of the NLP models.
* **Feature Engineering:** Analyzed user metadata such as `user_followers` and `user_verified` status.

---

## 🛠️ Natural Language Processing Pipeline

To transform raw tweets into a format suitable for AI, the following pipeline was implemented:

1. **Noise Removal:** Eliminated HTML tags, URLs, mentions (`@`), and special characters.
2. **Contraction Mapping:** Replaced shorthand (e.g., "don't" → "do not").
3. **Normalization:** Converted all text to lowercase and removed English stopwords.
4. **Tokenization & Lemmatization:** Reduced words to their root form (e.g., "watching" → "watch").
5. **Vectorization:** Converted text into numerical vectors using **TF-IDF / CountVectorizer**.

---

## 🚀 Machine Learning Models

We compared multiple supervised learning models to identify the most accurate sentiment predictor:

* **Logistic Regression** (Base Model)
* **Random Forest Classifier**
* **Multinomial Naive Bayes**

### Performance Metrics

The models were evaluated based on:

* **Accuracy Score**
* **Precision, Recall, and F1-Score**
* **Confusion Matrix** (to visualize misclassifications across the three sentiment categories)

---

## 💡 Findings & Visualizations

* **Key Themes:** A Wordcloud of the top 40 features reveals that users frequently discussed the "scary" and "eye-opening" nature of algorithmic influence.
* **Sentiment Distribution:** The analysis provides a clear breakdown of whether the global Twitter community viewed the documentary's warnings with alarm, agreement, or neutrality.

---

## ⚙️ How to Run

1. **Clone the repo:**
```bash
git clone https://github.com/YOUR_USERNAME/Social-Dilemma-Sentiment-Analysis.git

```


2. **Install dependencies:**
```bash
pip install pandas numpy matplotlib seaborn nltk sklearn

```


3. **Run the Notebook:**
Open `NLP_Project_Solution.ipynb` in Jupyter or VS Code to view the full analysis.

---

**Author:** [Your Name]

**Topic:** Statistical NLP | Media & Sentiment Analysis
