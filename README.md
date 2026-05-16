# Alexa-Review-Sentimental-Analysis
<img width="2480" height="1396" alt="image" src="https://github.com/user-attachments/assets/1125765f-9a7b-4c88-8380-59dce02f5104" />

## Project overflow

🛠️ Leveraging the Amazon Alexa customer reviews dataset available on Kaggle, we developed a sentiment classification model that categorizes input text as positive or negative. This model serves as a valuable tool for analyzing customer opinions and improving product quality based on user feedback.

📝 Our data preparation phase involved sophisticated text preprocessing techniques. We leveraged the **NLTK** library to perform **lemmatization**, reducing words to their base forms. Additionally, we employed vectorization to transform text into numerical features and utilized the **bag-of-words model** to capture term frequencies. This multi-faceted approach allowed us to extract meaningful features from the raw text reviews

📈 After training 𝐑𝐚𝐧𝐝𝐨𝐦 𝐅𝐨𝐫𝐞𝐬𝐭, **Logistic Regression**, **SVM**, 𝐃𝐞𝐜𝐢𝐬𝐢𝐨𝐧 𝐓𝐫𝐞𝐞𝐬, 𝐗𝐆𝐁𝐨𝐨𝐬𝐭, **Multilayer perceptron** and **Multinomial Naive bayes** models with optimal hyperparamter, we rigorously evaluated their performance with 𝐀𝐔𝐂-𝐑𝐎𝐂 𝐜𝐮𝐫𝐯𝐞𝐬 𝐚𝐧𝐝 𝐜𝐨𝐧𝐟𝐮𝐬𝐢𝐨𝐧 𝐦𝐚𝐭𝐫𝐢𝐜𝐞𝐬.

🎉 Excited to announce that our model boasts an impressive 𝟗3% 𝐚𝐜𝐜𝐮𝐫𝐚𝐜𝐲 𝐫𝐚𝐭𝐞, providing companies with actionable insights for product development and enhancing overall user experience

# Amazon Alexa Review - Sentiment Analysis

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
```

This converts customer reviews into numerical vectors based on the frequency of important words.

---

# 🤖 Machine Learning Models Used

The project trains and compares multiple machine learning models:

| Model | Purpose |
|---|---|
| Logistic Regression | Linear classification baseline |
| Random Forest Classifier | Ensemble learning model |
| Multinomial Naive Bayes | NLP-based probabilistic classifier |
| XGBoost Classifier | Gradient boosting model |

---

# 🔧 Hyperparameter Tuning

The project uses:

## GridSearchCV

for optimizing model performance.

### Tuned Parameters Include:

- Learning rate
- Max depth
- Number of estimators
- Regularization parameters
- Solver selection
- Alpha smoothing

Cross-validation is used for better model generalization.

---

# 📈 Model Evaluation Metrics

Models are evaluated using:

- Accuracy Score
- Precision Score
- Recall Score
- F1 Score
- ROC-AUC Score

---

# 🏆 Best Performing Model

## XGBoost Classifier (Tuned)

Among all the trained models, the tuned XGBoost Classifier achieved the best overall performance for sentiment classification.

### Why XGBoost performed best

- Handles sparse text features efficiently
- Works well with high-dimensional NLP data
- Provides better generalization
- Reduces overfitting using boosting techniques

---

# 🔄 Project Workflow

```text
Dataset Collection
        ↓
Data Cleaning
        ↓
Exploratory Data Analysis
        ↓
Text Preprocessing
        ↓
Feature Extraction using CountVectorizer
        ↓
Train-Test Split
        ↓
Model Training
        ↓
Hyperparameter Tuning
        ↓
Model Evaluation
        ↓
Sentiment Prediction
```

---

# 📁 Folder Structure

```bash
Amazon-Alexa-Review-Sentiment-Analysis/
│
├── Amazon Alexa Review - Sentiment Analysis.ipynb
├── amazon_alexa.tsv
├── README.md
└── requirements.txt
```

---

# 🚀 Installation

Clone the repository:

```bash
git clone https://github.com/Supratim0406/Alexa-Review-Sentimental-Analysis.git
```

Move into the project directory:

```bash
cd Alexa-Review-Sentimental-Analysis
```

Install dependencies:

```bash
pip install -r requirements.txt
```

---

# ▶️ Run the Project

Launch Jupyter Notebook:

```bash
jupyter notebook
```

Open the notebook:

```bash
Amazon Alexa Review - Sentiment Analysis.ipynb
```

---

# 📌 Key Insights

- More than 90% of reviews are positive.
- Positive reviews are generally longer and more descriptive.
- Product variation influences customer ratings.
- NLP preprocessing significantly improves classification performance.
- XGBoost outperformed traditional ML algorithms.

---

# 🔮 Future Improvements

Potential improvements for production deployment:

- Deploy using Streamlit or Flask
- Use TF-IDF Vectorization
- Integrate Deep Learning models (LSTM/GRU)
- Use Transformer models like BERT
- Dockerize the project
- Deploy on AWS/GCP/Azure
- Create REST APIs for inference

---

# 🎯 Skills Demonstrated

This project demonstrates practical knowledge of:

- Natural Language Processing (NLP)
- Text Cleaning & Preprocessing
- Exploratory Data Analysis
- Feature Engineering
- Machine Learning Classification
- Hyperparameter Tuning
- Model Evaluation
- Data Visualization

---

# 👨‍💻 Author

## Supratim Saha

- GitHub: https://github.com/Supratim0406
- LinkedIn: https://www.linkedin.com/in/itsmesupratim/

---

# 🔗 Repository Link

https://github.com/Supratim0406/Alexa-Review-Sentimental-Analysis

---

# ⭐ If you found this project useful, don't forget to give it a star on GitHub.
