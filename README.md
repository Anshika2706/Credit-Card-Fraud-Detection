# Credit-Card-Fraud-Detection
“A machine learning project for detecting fraudulent credit card transactions using Random Forest.”
💳 Credit Card Fraud Detection using Machine Learning
📌 Overview

The goal of this project is to develop a Machine Learning model that can accurately detect fraudulent credit card transactions.
By analyzing transaction patterns, the model distinguishes between legitimate and fraudulent activity — helping financial institutions reduce risks and losses.

📊 Dataset Information

Source: Kaggle Credit Card Fraud Detection Dataset

Records: ~2,84,000 transactions

Fraud Cases: 492

Nature: Highly imbalanced dataset

Description: The dataset contains real anonymized transactions made by European cardholders in 2013.
Each transaction includes features V1–V28 (PCA-transformed), along with Amount and Class (0 = Not Fraud, 1 = Fraud).

🤖 Model Used

Random Forest Classifier

Ensemble method combining multiple decision trees.

Handles non-linear relationships effectively.

Reduces overfitting through bagging.

Provides feature importance to understand which variables are most useful.

⚙️ Model Training and Evaluation

Data Split: 80% Training | 20% Testing

Evaluation Metrics Used:

Accuracy: 99.96% — Overall performance (but can be misleading for imbalanced data)

Precision: 98.73% — When model says “fraud,” it’s correct 98.7% of the time

Recall: 79.59% — Model catches ~80% of all actual frauds

F1-Score: 88.14% — Balance between precision & recall

MCC: 0.8863 — Balanced performance indicator even with class imbalance

📈 Visualizations

The following visualizations were used for data understanding:

Correlation heatmap of features

Feature importance plot

Fraud vs Non-Fraud transaction distribution

🧠 Key Insights

Features like V2 and V5 show negative correlation with the Amount feature.

The dataset is highly imbalanced, so metrics like precision, recall, and MCC are more reliable than accuracy.

Random Forest provides both high precision and good recall, making it an effective fraud detection model.

🧩 Future Improvements

Apply SMOTE or undersampling to handle class imbalance

Try XGBoost / LightGBM for better performance

Deploy model as a simple web app (Streamlit / Flask)

🛠️ Tech Stack

Language: Python

Libraries: pandas, numpy, matplotlib, seaborn, scikit-learn

Environment: Jupyter Notebook

📁 How to Run

Clone the repository

git clone https://github.com/AnshikaBhargava/Credit-Card-Fraud-Detection.git


Install dependencies

pip install -r requirements.txt


Run the Jupyter notebook

jupyter notebook fraud_detection.ipynb

✨ Author

Anshika Bhargava
3rd Year | B.Tech CSE
💼 Focus: Machine Learning & Data Science
