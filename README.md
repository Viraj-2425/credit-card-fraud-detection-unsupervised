💳 Credit Card Fraud Detection using Unsupervised Learning
📌 Project Overview

Fraudulent transactions in financial systems are rare and often unlabelled, making them difficult to detect using traditional supervised learning techniques. This project develops an Unsupervised Fraud Detection System using clustering and anomaly detection methods to identify suspicious credit card transactions.

The project follows a real-world scenario where fraud labels are unavailable during model training and are used only for evaluation.

🎯 Objectives
Understand the structure of the credit card transaction dataset.
Perform Exploratory Data Analysis (EDA).
Preprocess and scale transaction features.
Apply clustering and anomaly detection techniques.
Detect potentially fraudulent transactions.
Compare different unsupervised learning approaches.
Evaluate model performance using actual fraud labels.
📊 Dataset

Dataset: Credit Card Fraud Detection Dataset

Total Transactions: 284,807
Fraud Transactions: 492
Normal Transactions: 284,315
Features: 31
Target Variable: Class
0 → Legitimate Transaction
1 → Fraudulent Transaction

The dataset is highly imbalanced, with fraudulent transactions representing only 0.17% of all records.

🛠️ Technologies Used
Python
Jupyter Notebook
Pandas
NumPy
Matplotlib
Seaborn
Scikit-learn
📈 Exploratory Data Analysis

Performed:

Dataset inspection
Missing value analysis
Duplicate value detection
Fraud vs Normal transaction analysis
Transaction amount distribution
Correlation analysis
Class imbalance visualization
⚙️ Data Preprocessing
Removed duplicate records
Selected relevant features
Excluded fraud labels during training
Standardized features using StandardScaler
🤖 Models Implemented
1️⃣ K-Means Clustering

Used K-Means to group transactions into clusters and identify abnormal patterns.

Advantages

Simple and fast
Easy to interpret

Limitations

Sensitive to class imbalance
Assumes spherical clusters
2️⃣ Isolation Forest

Used Isolation Forest to identify anomalous transactions.

Advantages

Designed specifically for anomaly detection
Effective on imbalanced datasets
Scalable for large datasets

Limitations

Requires contamination parameter tuning
📋 Evaluation Metrics

Actual fraud labels were used only after model training.

Metrics evaluated:

Confusion Matrix
Precision
Recall
F1 Score

Key Findings
Fraudulent transactions are extremely rare.
K-Means struggled to separate fraud transactions effectively.
Isolation Forest detected anomalies more accurately.
Unsupervised learning can successfully identify suspicious transactions without relying on labelled training data.
