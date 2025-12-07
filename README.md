# 🌟 LGD Prediction Using Apache Spark  
### *Credit Risk Modeling • Machine Learning • Big Data • Visual Analytics*

<p align="center">
  <img src="https://img.shields.io/badge/Spark-3.4.2-orange?logo=apache-spark&logoColor=white" />
  <img src="https://img.shields.io/badge/PySpark-MLlib-blue?logo=python&logoColor=white" />
  <img src="https://img.shields.io/badge/Python-3.10-green?logo=python" />
  <img src="https://img.shields.io/badge/Jupyter-Notebook-orange?logo=jupyter" />
  <img src="https://img.shields.io/badge/EDA-Visualizations-purple" />
</p>

---

## 📘 Project Overview

This repository contains a complete **LGD (Loss Given Default) prediction workflow** built with **Apache Spark** and supported by a second notebook for **visual exploration and insights**.

The project includes:

- Scalable Spark-based data preprocessing  
- Advanced feature engineering  
- ML model pipeline for LGD prediction  
- Model evaluation  
- Deployment prediction  
- Rich exploratory visualizations (Matplotlib, Seaborn)  

---

# 🚀 Notebook 1: LGD_Prediction_Spark.ipynb  
### *Spark-Based Data Processing & Machine Learning Pipeline*

This notebook performs the entire modeling pipeline using **PySpark**:

### 🔍 **Data Preparation**
- Clean numeric formatting (`,` → `.`)
- Convert columns to numeric types  
- Handle missing values  
- Outlier correction using IQR method  

### 🧠 **Feature Engineering**
Using Spark Window Functions:

- `Defaults_mean_by_Credit_Score`
- `Income_mean_by_Region`

### 🤖 **Machine Learning Pipeline**
Built using Spark MLlib:

- `StringIndexer`
- `OneHotEncoder`
- `VectorAssembler`
- `StandardScaler`
- `LinearRegression`

### 📈 **Model Performance**

| Metric | Train | Test |
|--------|--------|---------|
| **MAE** | ~0.118 | ~0.118 |
| **RMSE** | ~0.145 | ~0.144 |
| **R²** | ~0.820 | ~0.824 |

The model demonstrates strong generalization and excellent predictive capability for credit LGD.

### 🔮 **Deployment**
The trained pipeline is applied to a second dataset to generate **LGD predictions for new loan applicants**.

---

# 📊 Notebook 2: Visuals-new.ipynb  
### *Comprehensive EDA & Visual Insights*

This notebook contains **visualizations and statistical insights** using Pandas, Matplotlib, and Seaborn.

### 📌 Included Plots:
- Distribution plots for key numeric variables  
- Boxplots to identify outliers  
- Heatmap of feature correlations  
- LGD distribution analysis  
- Scatterplots of LGD vs predictors  
- Categorical variable bar charts  
- Pairwise relationships  

### 🎯 Purpose of the Visuals Notebook
- Understand variable behavior  
- Support feature engineering decisions  
- Identify non-normal distributions  
- Highlight important predictors  
- Provide material for reporting & presentations  

The visuals complement the Spark ML notebook by offering clarity and intuition behind the modeling strategy.




