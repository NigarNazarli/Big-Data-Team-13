# Big-Data-Team-13
🌟 LGD Prediction Using Apache Spark
Credit Risk Modeling • Machine Learning • Big Data Processing
<p align="center"> <img src="https://img.shields.io/badge/Spark-3.4.2-orange?logo=apache-spark&logoColor=white" /> <img src="https://img.shields.io/badge/PySpark-MLlib-blue?logo=python&logoColor=white" /> <img src="https://img.shields.io/badge/Python-3.10-green?logo=python" /> <img src="https://img.shields.io/badge/Jupyter-Notebook-orange?logo=jupyter" /> </p>
📘 Project Overview

This project implements an end-to-end Loss Given Default (LGD) prediction model using Apache Spark MLlib, enabling efficient large-scale credit-risk modeling.

The notebook performs:

Data loading & cleaning

Outlier treatment

Feature engineering with window functions

Encoding & scaling

Spark ML linear regression

Performance evaluation

Deployment predictions

The final model predicts LGD for new loan observations with high generalization accuracy.

⚙️ Technologies Used

Apache Spark 3.4.x

PySpark SQL + MLlib

Python 3.10

Pandas (for EDA sections)

SciPy / NumPy

Jupyter Notebook

📂 Repository Structure
📁 project/
│
├── LGD_Prediction_Spark.ipynb     # Main notebook (Spark implementation)
├── lgd_data.csv                   # Training dataset
├── lgd_deploy.csv                 # Deployment dataset
└── README.md                      # Project documentation

🚀 Key Features
🔍 1. Data Preprocessing

Handles missing values

Normalizes European decimal formatting (, → .)

Converts numeric columns to proper types

Removes extreme outliers using IQR

🧠 2. Feature Engineering

Mean defaults per credit score

Mean income per region

Additional statistical enrichments using Spark’s Window functions

🤖 3. Machine Learning Pipeline

Implemented using Spark MLlib Pipeline API:

StringIndexer

OneHotEncoder

VectorAssembler

StandardScaler

LinearRegression

📈 4. Evaluation

Metrics reported:

Metric	Train	Test
MAE	~0.118	~0.118
RMSE	~0.145	~0.144
R²	~0.820	~0.824

➡️ High generalization and strong predictive performance.

🔮 5. Deployment Phase

A separate dataset is processed through the same pipeline to generate:

Predicted LGD values for new loans.

🛠️ How to Run
1️⃣ Install Dependencies
pip install pyspark pandas numpy scipy notebook

2️⃣ Start Jupyter
jupyter notebook

3️⃣ Open the Notebook & Run All Cells

Make sure:

Spark is installed (v3.4.x)

Java 8 is configured

File paths match your local environment

📊 Notebook Workflow
1. Load dataset (CSV)
2. Clean numeric formatting & handle missing values
3. Outlier removal (IQR)
4. Feature engineering using Spark Window functions
5. Categorical encoding and feature scaling
6. Train-test split
7. Linear Regression training
8. Evaluation (MAE, RMSE, R²)
9. Deployment predictions
10. Pandas-based EDA (optional)

🧪 Output (Model Performance)
Train MAE: 0.11797
Train RMSE: 0.14459
Train R2: 0.81975

Test MAE: 0.11768
Test RMSE: 0.14407
Test R2: 0.82420
