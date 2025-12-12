# ml-fake-job-detection-project
🌐 Fake Job Detection using Machine Learning

A machine learning project that identifies fraudulent job postings using NLP, data cleaning, and a Random Forest classifier.

📁 Repository: ml-fake-job-detection-project
📌 Project Overview

Fake job posts have become increasingly common on job portals. This project builds a predictive model that analyzes job descriptions and metadata to classify whether a job posting is real or fraudulent.

This model can help job seekers, HR platforms, and researchers understand the patterns behind fake job listings.

📂 Dataset

The dataset used is the Real/Fake Job Posting Dataset from Kaggle.

Features include:

Job title, location

Department, salary range

Company profile

Job description, requirements

Telecommuting, employment type, benefits

Fraudulent label (0 = Real, 1 = Fake)

🧹 Data Preprocessing

Key preprocessing steps performed:

Removed irrelevant/unstructured columns

Cleaned null values

Combined text fields where required

Lowercased text

Removed punctuation, stopwords

Tokenization & Lemmatization

TF-IDF vectorization for text fields

Handled class imbalance if present

Train-test split (80/20)

🤖 Model Used: Random Forest Classifier

Random Forest was chosen because:

Works well with high-dimensional text data

Reduces overfitting via multiple decision trees

Good accuracy on classification problems

Handles non-linear patterns

📊 Model Performance
✔ Confusion Matrix (Example)
[[5103     2]
 [ 159   100]]

✔ Interpretation:

True Negatives (5103): Real jobs correctly identified as real

False Positives (2): Real jobs incorrectly predicted as fake

False Negatives (159): Fake jobs wrongly predicted as real

True Positives (100): Fake jobs correctly identified as fake

✔ Meaning:

The model is very good at detecting real jobs

It struggles more with detecting fake jobs, because fake listings are rare → dataset imbalance

Still, the model successfully identifies patterns of fraudulent postings

📈 Metrics

(Replace with your actual values if needed)

Accuracy: ~95%

Precision: High for class 0

Recall: Lower for fake class

F1-score: Balanced

🏗 Project Structure
ml-fake-job-detection-project/
│── dataset/
│     └── fake_job_postings.csv
│── notebooks/
│     └── fake_job_detection.ipynb
│── README.md

▶️ How to Run the Project
1️⃣ Clone the repo
git clone https://github.com/<your-username>/ml-fake-job-detection-project.git
cd ml-fake-job-detection-project

2️⃣ Install requirements
pip install -r requirements.txt

3️⃣ Run the notebook

Open Jupyter Notebook:

jupyter notebook


Run fake_job_detection.ipynb

🚀 Future Improvements

Use BERT embeddings for better text understanding

Handle class imbalance with SMOTE

Deploy model with Flask / FastAPI

Add a frontend dashboard

Create real-time prediction API

📝 Author

Vinay N.
Machine Learning & Data Science Enthusiast
