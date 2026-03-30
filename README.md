# 📩 Email / SMS Spam Classifier (End-to-End ML + Streamlit Deployment)

A complete machine learning project that builds and deploys a **spam classification system** for email/SMS messages using NLP, TF-IDF, and a trained ML model.

This project demonstrates the **full ML lifecycle**, from data preprocessing to real-time deployment via Streamlit.

---

## 🚀 Project Overview

This system classifies messages as **Spam or Not Spam** using:

- NLP preprocessing techniques  
- TF-IDF feature extraction  
- Machine learning classification  
- Streamlit-based interactive deployment  

The workflow follows:

> **Data → Preprocessing → Feature Engineering → Model Training → Serialization → Deployment**

---

## 🌐 Live Application

👉 **Deployed App:**  
https://jcrshgvw7rwfzwhtvbrzfo.streamlit.app/

---

## 🎯 Objectives

- Build a robust text classification pipeline  
- Apply NLP preprocessing techniques  
- Train and evaluate a spam detection model  
- Deploy a real-time prediction system using Streamlit  

---

## 🧠 Core Concepts Covered

- Text preprocessing:
  - lowercasing  
  - tokenization (NLTK)  
  - stopword removal  
  - stemming (Porter Stemmer)  

- Feature Engineering:
  - TF-IDF vectorization  

- Machine Learning:
  - text classification model  

- Deployment:
  - model serialization (`.pkl`)  
  - Streamlit-based UI  

---

## 📂 Project Structure

```
EMAIL_SPAM_CLASSIFIER/
│
├── app.py                      # Streamlit web application
├── sms_spam_detection.ipynb    # Model training pipeline
│
├── spam.csv                    # Dataset
│
├── model.pkl                   # Trained model
├── vectorizer.pkl              # TF-IDF vectorizer
│
├── requirements.txt
├── LICENSE
├── README.md
└── .gitignore
```

---

## ⚙️ How It Works

### 1️⃣ Text Preprocessing

- Tokenization  
- Removal of punctuation and stopwords  
- Stemming  

```python
transform_text(text)
```

---

### 2️⃣ Feature Transformation

```python
vector_input = tfidf.transform([processed_text])
```

- Converts text into numerical vectors  
- Uses pre-trained TF-IDF vocabulary  

---

### 3️⃣ Prediction

```python
result = model.predict(vector_input)
```

- Output:
  - `1 → Spam`  
  - `0 → Not Spam`  

---

### 4️⃣ Streamlit Interface

- User inputs message  
- Model returns prediction instantly  

---

## 📊 Model Performance

*(Based on notebook evaluation)*

- Accuracy: ~97%  
- Precision: ~92%  

**Focus:** High precision to reduce false spam classification  

---

## 🛠 Installation

### Clone repository

```bash
git clone https://github.com/RudrTyagi1135/email_spam_classifier.git
cd email_spam_classifier
```

### Install dependencies

```bash
pip install -r requirements.txt
```

---

## ▶️ Run the Project

```bash
streamlit run app.py
```

---

## ⚠️ Important Notes

### Model Consistency

- `model.pkl` and `vectorizer.pkl` must come from the same training run  
- Mismatch → feature dimension errors  

---

### Preprocessing Consistency

- Same preprocessing must be used in:
  - training notebook  
  - deployment (`app.py`)  

---

### NLTK Dependencies

```python
nltk.download('punkt')
nltk.download('stopwords')
```

---

## ⚠️ Limitations

- No cross-validation  
- No model comparison  
- Separate vectorizer and model (risk of mismatch)  
- No pipeline abstraction  

---

## 🔮 Future Improvements

- Use **Pipeline (TF-IDF + Model)** for safer deployment  
- Add evaluation metrics:
  - F1 Score  
  - ROC-AUC  
- Compare models:
  - Naive Bayes  
  - Logistic Regression  
  - SVM  
- Improve NLP:
  - Lemmatization  
  - N-grams  
- Deploy using:
  - Docker  
  - FastAPI backend  
  - AWS / GCP  

---

## 📊 Outputs

- Spam classification predictions  
- Real-time inference via web interface  
- Serialized ML artifacts for deployment  

---

## 🎯 What This Project Demonstrates

- End-to-end ML system design  
- NLP preprocessing and feature engineering  
- Model deployment using Streamlit  
- Handling training vs inference consistency  

---

## 📌 Next Step

- Convert into production ML pipeline  
- Add model monitoring and logging  
- Build API-based inference system  
- Integrate into MLOps workflow  

---

## 👤 Author

**Rudra Tyagi**

ML Systems | MLOps | AI Infrastructure
