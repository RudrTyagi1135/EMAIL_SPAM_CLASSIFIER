# 📉 Principal Component Analysis (PCA): From Linear Algebra to Dimensionality Reduction

## 🔍 Overview

This project provides a **deep, mathematical and practical exploration of Principal Component Analysis (PCA)**, covering:

* Step-by-step manual implementation
* Eigen decomposition and covariance analysis
* Singular Value Decomposition (SVD)
* Practical dimensionality reduction using sklearn

The goal is to move from:

> **“using PCA” → “understanding the linear algebra that powers dimensionality reduction”**

---

## 🎯 Objectives

* Build PCA **from first principles**
* Understand:

  * covariance matrix
  * eigenvalues and eigenvectors
* Connect PCA with **Singular Value Decomposition (SVD)**
* Apply PCA for:

  * dimensionality reduction
  * feature transformation

---

## 🧠 Core Concepts Covered

* Mean centering of data
* Covariance matrix
* Eigen decomposition
* Principal components
* Explained variance
* Singular Value Decomposition (SVD)
* Dimensionality reduction

---

## 🏗️ Project Structure

```bash id="q8o7px"
PCA/
│
├── pca_step_by_step.ipynb              # Manual PCA implementation
├── pca_variants.ipynb                 # PCA using sklearn + experiments
├── singular_value_decomposition.ipynb # SVD foundation of PCA
│
├── README.md
├── requirements.txt
├── LICENSE
└── .gitignore
```

---

## ⚙️ Implementation Breakdown

### 1️⃣ PCA from Scratch (Step-by-Step)

* Steps implemented manually:

  1. Mean centering
  2. Covariance matrix computation
  3. Eigenvalue and eigenvector calculation
  4. Sorting components by variance
  5. Projection onto principal components

📌 **Key Insight:**

* Principal components represent directions of maximum variance

---

### 2️⃣ PCA Variants (Practical Usage)

* Uses sklearn PCA
* Demonstrates:

  * dimensionality reduction
  * explained variance ratio
  * effect of number of components

📌 **Key Insight:**

* PCA reduces dimensionality while preserving maximum information

---

### 3️⃣ Singular Value Decomposition (SVD)

* Implements SVD:
  [
  X = U \Sigma V^T
  ]

* Connects SVD to PCA

📌 **Key Insight:**

* PCA can be computed efficiently using SVD
* SVD is numerically more stable

---

## 📊 Key Observations

### 📉 Dimensionality Reduction

* Reduces feature space while retaining most variance
* Helps with:

  * visualization
  * noise reduction
  * faster computation

---

### 📈 Explained Variance

* First few components capture majority of information
* Remaining components contribute minimal variance

---

### ⚠️ Information Loss

* Reducing dimensions leads to:

  * loss of some information
* Trade-off between:

  * compression
  * accuracy

---

## ⚠️ Limitations

* No pipeline integration with ML models
* No visualization of variance explained curve (scree plot)
* No comparison with other dimensionality reduction methods
* No real-world dataset evaluation
* Assumes linear relationships

---

## 🚀 Future Improvements (High-Impact)

To elevate this into a **production-grade ML preprocessing component**:

* Add **Scree Plot (explained variance curve)**
* Integrate PCA into:

  * classification pipeline
  * regression pipeline
* Compare with:

  * t-SNE
  * UMAP
* Apply on **real-world high-dimensional dataset**
* Add **feature scaling before PCA (critical)**

---

## 🧪 How to Run

```bash id="j3n8yt"
# Clone repository
git clone https://github.com/RudrTyagi1135/PCA.git

# Navigate to project
cd PCA

# Install dependencies
pip install -r requirements.txt

# Run notebooks
jupyter notebook
```

---

## 📌 Key Takeaways

* PCA is a **linear algebra-driven technique** for dimensionality reduction

* Understanding eigen decomposition and SVD is essential for:

  * efficient computation
  * numerical stability

* PCA is widely used in:

  * preprocessing pipelines
  * feature engineering
  * visualization

---

## 👨‍💻 Author

**Rudra Tyagi**
Aspiring ML Systems / MLOps Engineer

* GitHub: https://github.com/RudrTyagi1135

---

## ⭐ Support

If this project helped you understand PCA deeply, consider starring ⭐ the repository.
