# Alexa-Review-Sentimental-Analysis
<img width="2480" height="1396" alt="image" src="https://github.com/user-attachments/assets/1125765f-9a7b-4c88-8380-59dce02f5104" />

## Project overflow

🛠️ Leveraging the Amazon Alexa customer reviews dataset available on Kaggle, we developed a sentiment classification model that categorizes input text as positive or negative. This model serves as a valuable tool for analyzing customer opinions and improving product quality based on user feedback.

📝 Our data preparation phase involved sophisticated text preprocessing techniques. We leveraged the **NLTK** library to perform **lemmatization**, reducing words to their base forms. Additionally, we employed vectorization to transform text into numerical features and utilized the **bag-of-words model** to capture term frequencies. This multi-faceted approach allowed us to extract meaningful features from the raw text reviews

📈 After training 𝐑𝐚𝐧𝐝𝐨𝐦 𝐅𝐨𝐫𝐞𝐬𝐭, **Logistic Regression**, **SVM**, 𝐃𝐞𝐜𝐢𝐬𝐢𝐨𝐧 𝐓𝐫𝐞𝐞𝐬, 𝐗𝐆𝐁𝐨𝐨𝐬𝐭, **Multilayer perceptron** and **Multinomial Naive bayes** models with optimal hyperparamter, we rigorously evaluated their performance with 𝐀𝐔𝐂-𝐑𝐎𝐂 𝐜𝐮𝐫𝐯𝐞𝐬 𝐚𝐧𝐝 𝐜𝐨𝐧𝐟𝐮𝐬𝐢𝐨𝐧 𝐦𝐚𝐭𝐫𝐢𝐜𝐞𝐬.

🎉 Excited to announce that our model boasts an impressive 𝟗3% 𝐚𝐜𝐜𝐮𝐫𝐚𝐜𝐲 𝐫𝐚𝐭𝐞, providing companies with actionable insights for product development and enhancing overall user experience

from pathlib import Path

readme_content = r"""# Amazon Alexa Review - Sentiment Analysis

An end-to-end Natural Language Processing (NLP) and Machine Learning project that analyzes Amazon Alexa customer reviews and predicts whether the sentiment is positive or negative.

This project demonstrates a complete real-world NLP workflow including:

- Data Cleaning & Preprocessing
- Exploratory Data Analysis (EDA)
- Text Processing using NLP
- Feature Engineering using CountVectorizer
- Machine Learning Model Training
- Hyperparameter Tuning
- Model Evaluation & Comparison
- Sentiment Prediction

---

# 📌 Project Overview

Customer reviews contain valuable insights about user satisfaction and product experience.

In this project, Amazon Alexa product reviews are analyzed using Natural Language Processing (NLP) techniques and multiple Machine Learning algorithms to classify customer sentiment.

The project includes:

- Exploratory analysis of customer reviews
- Text preprocessing and cleaning
- WordCloud visualization
- Feature extraction from text data
- Training multiple ML models
- Hyperparameter tuning using GridSearchCV
- Model comparison using evaluation metrics

---

# 📂 Dataset Information

The dataset contains Amazon Alexa product reviews.

## Features

| Feature | Description |
|---|---|
| rating | Product rating given by customer |
| date | Date of review |
| variation | Product variation/model |
| verified_reviews | Customer review text |
| feedback | Sentiment label (0 = Negative, 1 = Positive) |

## Target Variable

- `0` → Negative Review
- `1` → Positive Review

## Business Logic Used

- Ratings `1` and `2` are treated as Negative Reviews
- Ratings `3`, `4`, and `5` are treated as Positive Reviews

---

# 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- NLTK
- XGBoost
- WordCloud
- Jupyter Notebook

---

# 📊 Exploratory Data Analysis (EDA)

The project performs detailed exploratory data analysis including:

## Rating Distribution

- Count plots
- Pie charts
- Histogram visualization

## Feedback Analysis

- Positive vs Negative review distribution
- Sentiment percentage analysis

## Variation Analysis

- Product variation frequency
- Average rating by product variation
- Feedback comparison across variations

## Review Length Analysis

- Review length distribution
- Review length comparison for positive and negative reviews

## WordCloud Visualization

Generated separate WordClouds for:

- Positive Reviews
- Negative Reviews

### Common Positive Words

- good
- amazing
- great
- best
- excellent

### Common Negative Words

- horrible
- garbage
- poor
- disappointing

---

# 🧹 NLP Preprocessing Pipeline

The review text is cleaned and preprocessed using the following techniques:

1. Lowercase conversion
2. Removing special characters
3. Removing punctuation
4. Removing stopwords
5. Tokenization
6. Stemming using PorterStemmer
7. Lemmatization using WordNetLemmatizer

---

# ⚙️ Feature Engineering

The project uses:

## CountVectorizer

```python
CountVectorizer(max_features=2500)
