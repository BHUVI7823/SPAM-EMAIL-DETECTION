# 📧 Spam Email Detection using Machine Learning

## 📌 Project Overview

This project aims to classify emails as **Spam** or **Ham (Not Spam)** using Machine Learning and Natural Language Processing (NLP). The model preprocesses email text, converts it into numerical features using Bag of Words, and predicts whether an email is spam.

---

## 🎯 Objectives

- Detect spam emails automatically.
- Perform text preprocessing using NLP techniques.
- Convert text into numerical vectors using CountVectorizer.
- Train multiple machine learning models.
- Optimize Random Forest using GridSearchCV.
- Evaluate model performance using various metrics.

---

## 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- NLTK
- Scikit-learn
- Regular Expressions (Regex)

---

## 📚 Libraries Used

```python
pandas
numpy
nltk
re
scikit-learn
```

---

## 📂 Dataset

The dataset contains:

- Email Text
- Spam Label

Target Variable:

- **0 → Ham (Not Spam)**
- **1 → Spam**

---

## 🔍 Data Preprocessing

The following preprocessing steps were performed:

- Removed special characters using Regular Expressions
- Converted text to lowercase
- Tokenization
- Removed stopwords
- Applied Porter Stemming
- Created Bag of Words using CountVectorizer

---

## 🧠 Feature Extraction

Used **CountVectorizer**

```python
CountVectorizer(max_features=1600)
```

This converts email text into numerical feature vectors.

---

## 🤖 Machine Learning Models

The following models were implemented:

- Gaussian Naive Bayes
- Random Forest Classifier

Random Forest hyperparameters were optimized using **GridSearchCV**.

---

## ⚙️ Hyperparameter Tuning

Parameters used:

- n_estimators
- criterion
- max_depth

GridSearchCV was used to find the best combination.

---

## 📊 Model Evaluation

Evaluation metrics:

- Accuracy Score
- Confusion Matrix
- Classification Report

Example Results:

- **Training Accuracy:** 97.09%
- **Testing Accuracy:** 94.42%

Confusion Matrix:

```
[[841  44]
 [ 20 241]]
```

---

## 📈 Workflow

```
Dataset
     │
     ▼
Text Cleaning
     │
     ▼
Tokenization
     │
     ▼
Stopword Removal
     │
     ▼
Stemming
     │
     ▼
CountVectorizer
     │
     ▼
Train-Test Split
     │
     ▼
Model Training
     │
     ▼
Prediction
     │
     ▼
Performance Evaluation
```

---

## 📁 Project Structure

```
Spam Email Detection/
│
├── Spam_Email_Detection.ipynb
├── emails.csv
├── README.md
└── requirements.txt
```

---

## 🚀 How to Run

1. Clone the repository

```
git clone https://github.com/yourusername/Spam-Email-Detection.git
```

2. Install dependencies

```
pip install -r requirements.txt
```

3. Run the Jupyter Notebook

```
jupyter notebook
```

4. Open

```
Spam_Email_Detection.ipynb
```

---

## 📌 Sample Prediction

### Spam

```
Urgent! Your bank account has been suspended. Verify your details immediately.
```

Prediction:

```
Spam
```

### Ham

```
Hi John, let's meet tomorrow at 10 AM to discuss the project.
```

Prediction:

```
Ham
```

---

## 🌟 Future Improvements

- TF-IDF Vectorization
- Word Embeddings (Word2Vec, GloVe)
- Deep Learning using LSTM
- BERT-based Spam Detection
- Web Application using Streamlit or Flask

---

## 👩‍💻 Author

**Bhuvana Nagarajan**

Hindusthan Institute of Technology

---

## 📜 License

This project is developed for educational and learning purposes.
