# 🌐 Fake Job Detection using Machine Learning

A machine learning project that identifies fraudulent job postings using NLP, data cleaning, and a Random Forest classifier.

---

## 📁 Repository
**ml-fake-job-detection-project**

---

## 📌 Project Overview

Fake job posts are increasing across job portals.  
This project analyzes job descriptions and metadata to classify whether a job post is **real or fraudulent**.

It helps:
- Job seekers avoid scams  
- HR platforms flag suspicious postings  
- Researchers study fraud patterns  

---

## 📂 Dataset

Dataset used: **Real/Fake Job Posting Dataset (Kaggle)**

🔗 **Dataset is available here:**  
https://drive.google.com/drive/folders/10oAbFEyOf_fF8ZeHnFJ3w69fryncmkAM?usp=sharing

**Features include:**
- Job title  
- Location & department  
- Salary range  
- Company profile  
- Job description  
- Requirements  
- Benefits  
- Telecommuting, employment type  
- Target: `fraudulent` (0 = Real, 1 = Fake)

---

## 🧹 Data Preprocessing

Steps performed:
- Removed irrelevant/unstructured columns  
- Cleaned missing values  
- Merged text fields  
- Lowercased all text  
- Removed punctuation & stopwords  
- Tokenization + Lemmatization  
- TF-IDF vectorization  
- Handled class imbalance  
- Train-test split (80/20)

---

## 🤖 Model Used — Random Forest Classifier

**Why Random Forest?**
- Works well with high-dimensional text data  
- Reduces overfitting  
- High accuracy on classification tasks  
- Handles nonlinear patterns  

---

## 📊 Model Performance

### ✔ Confusion Matrix
[[5103 2]
[ 159 100]]



### ✔ Interpretation
- **True Negatives (5103)** → Real jobs correctly identified  
- **False Positives (2)** → Real jobs incorrectly marked as fake  
- **False Negatives (159)** → Fake jobs predicted as real  
- **True Positives (100)** → Fake jobs correctly detected  

### ✔ Meaning
- Excellent performance on real job detection  
- Harder to detect fake jobs → class imbalance issue  
- Still captures key fraud patterns well  

---

## 📈 Metrics
(Replace with your actual values)

- **Accuracy:** ~95%  
- **Precision:** High for class 0  
- **Recall:** Lower for fake jobs  
- **F1-Score:** Balanced  

---

## 🏗 Project Structure
ml-fake-job-detection-project/
│──G-Drive Link (dataset) - https://drive.google.com/drive/folders/10oAbFEyOf_fF8ZeHnFJ3w69fryncmkAM?usp=sharing
│── notebooks/
│ └── fake_job_detection.ipynb
│── README.md

---

## ▶️ How to Run the Project

### 1️⃣ Clone the repo
```bash
git clone https://github.com/<your-username>/ml-fake-job-detection-project.git
cd ml-fake-job-detection-project
2️⃣ Install dependencies
bash
Copy code
pip install -r requirements.txt
3️⃣ Run the notebook
bash
Copy code
jupyter notebook
Open fake_job_detection.ipynb

🚀 Future Improvements
Use BERT / Transformer-based embeddings

Apply SMOTE for class imbalance

Deploy using Flask / FastAPI

Build a prediction dashboard

Add interactive data visualizations

📝 Author
Vinay N.
Machine Learning & Data Science Enthusiast
