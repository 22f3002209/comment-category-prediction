# Comment Category Prediction

## 📌 Overview
This project focuses on building a machine learning model to classify user-generated comments into predefined categories. The task involves leveraging both textual data and additional structured features to improve prediction accuracy.

The goal is to develop a robust multi-class classification system that performs well on unseen data.

---

## 🎯 Objectives
- Perform data cleaning and preprocessing
- Conduct Exploratory Data Analysis (EDA)
- Handle missing values and feature imbalance
- Extract meaningful features from text data
- Build and evaluate machine learning models
- Improve prediction accuracy using combined features

---

## 📊 Dataset Description
The dataset consists of:
- **Text Data**
  - `comment` (user-generated text)

- **Numerical Features**
  - Engagement metrics: `upvote`, `downvote`
  - Internal features: `if_1`, `if_2`
  - Emoticon-related features: `emoticon_1`, `emoticon_2`, `emoticon_3`

- **Categorical Features**
  - `race`, `religion`, `gender`

- **Boolean Feature**
  - `disability`

- **Target Variable**
  - `label` (multi-class: 0 to 3)

---

## 🔍 Exploratory Data Analysis (EDA)

### Key Observations:
- Dataset contains a mix of numerical, categorical, and text features
- High missing values (~73%) in:
  - `race`, `religion`, `gender`
- Text data (`comment`) is mostly complete
- Comment lengths are **right-skewed**
- Most comments are short (0–300 characters)
- Longer comments tend to belong to specific classes
- User activity peaks during **evening hours (18–23)**
- Low correlation among features → model needs feature combination

---

## 🛠️ Data Preprocessing
- Handling missing values
- Encoding categorical variables
- Feature scaling (if applicable)
- Text preprocessing:
  - Lowercasing
  - Removing punctuation
  - Tokenization
  - Vectorization (TF-IDF)

---

## 🤖 Model Building
- Multi-class classification approach
- Models used:
  - Logistic Regression
  - SVM
  - Gradient Boosting (LGBM)
---

## 📈 Evaluation Metrics
- Accuracy 0.91
- Precision 0.81
- Recall 0.81
- F1-score 0.81

---

## 🚀 Key Insights
- Text data plays a crucial role in prediction
- Comment length is a useful feature
- Engagement metrics add predictive value
- Combining structured + unstructured data improves performance

---

## 📂 Project Structure
```
comment_category_prediction.ipynb   # Main notebook
README.md                           # Project documentation
```

---

## 🔧 Tech Stack
- Python
- Pandas & NumPy
- Scikit-learn
- Matplotlib / Seaborn
- NLP techniques

---

## 📌 Future Improvements
- Use deep learning models (LSTM, Transformers)
- Apply advanced NLP embeddings (BERT, Word2Vec)
- Hyperparameter tuning
- Better handling of missing categorical data

---

## 🙌 Conclusion
This project demonstrates how combining text data with structured features can significantly enhance classification performance. It highlights the importance of feature engineering, EDA, and thoughtful model selection in solving real-world machine learning problems.

---
