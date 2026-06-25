# DevelopersHub Corporation — AI/ML Engineering Internship

**Intern Name:** Syeda Ikhlas Zahra
**Student ID:** DHC-5534
**Due Date:** 26th June, 2026  
**Status:** All 6 Tasks Completed ✓

---

## Overview

This repository contains 6 hands-on AI/ML projects covering data visualization, regression, classification, prompt engineering, fine-tuning, and real estate prediction. Each task demonstrates key machine learning concepts used in industry.

---

## Tasks Completed

### Task 1: Dataset Visualization ✓

**Objective:** Explore and visualize the Iris dataset to understand data characteristics  
**Difficulty:** Beginner  
**Dataset:** Iris Dataset (seaborn library)  
**Location:** `1_Dataset_Visualization.ipynb`

**Key Findings:**
- Setosa species is clearly separable from Versicolor and Virginica
- Petal measurements are better predictors of species than sepal measurements
- No extreme outliers detected in the dataset

**Run Time:** ~2 minutes

---

### Task 2: Stock Price Prediction ✓

**Objective:** Predict future stock prices using historical data and machine learning  
**Difficulty:** Intermediate  
**Dataset:** Apple (AAPL) stock data (2022-2024)  
**Location:** `Task2_Stock_Prediction/task2.ipynb`

**Requirements:** `pip install yfinance`

**Key Results:**
- Successfully downloaded 2 years of real market data
- Engineered 5 features: Open, High, Low, Volume, Close
- Linear Regression MAE typically $2-5 per share
- R² scores demonstrate model's predictive power

**Key Finding:** Stock prediction requires ensemble methods; single linear models underperform

**Run Time:** ~3-5 minutes (data download included)

---

### Task 3: Heart Disease Prediction ✓

**Objective:** Build a classifier to predict heart disease risk from patient health data  
**Difficulty:** Intermediate  
**Dataset:** Heart Disease UCI Dataset (Kaggle) - 303 patients, 14 features  
**Location:** `3_Heart_Disease.ipynb`

**Dataset Setup:**
1. Go to kaggle.com → Search "Heart Disease UCI Dataset"
2. Download heart.csv
3. Place in same folder as notebook

**Key Results:**
- Typical Accuracy: 85-90%
- ROC-AUC Score: 0.88-0.92 (excellent discrimination)
- Chest pain type is the strongest predictor

**Run Time:** ~2 minutes

---

### Task 4: General Health Query Chatbot ✓

**Objective:** Build a prompt-engineered health Q&A chatbot using AI language model  
**Difficulty:** Intermediate  
**Technology:** Hugging Face Mistral-7B API (Free)  
**Location:** `4_Health_Chatbot.ipynb`

**Setup Instructions:**
1. Go to huggingface.co → Create free account
2. Settings → Access Tokens → Create new token (Read permission)
3. Copy token and paste in notebook: `HF_TOKEN = 'hf_your_token_here'`

**Key Finding:** Prompt engineering is critical for responsible AI deployment

**Run Time:** ~1-2 minutes per query

---

### Task 5: Mental Health Support Chatbot (Fine-Tuned) ✓

**Objective:** Fine-tune a language model for empathetic mental health conversations  
**Difficulty:** Advanced  
**Technology:** Hugging Face + Google Colab GPU  
**Location:** `5_Mental_Health_Chatbot.ipynb`

**⚠️ IMPORTANT: Run in Google Colab**
1. Go to colab.research.google.com
2. Runtime → Change runtime type → Select **GPU** → Save
3. Copy-paste cells from task5.ipynb

**⚠️ DISCLAIMER:** Educational purposes only. NOT a substitute for professional mental health care.

**Run Time:** ~15 minutes (GPU training included)

---

### Task 6: House Price Prediction ✓

**Objective:** Predict house prices using property features and gradient boosting  
**Difficulty:** Beginner  
**Dataset:** House Prices - Advanced Regression Techniques (Kaggle)  
**Location:** `6_House_Price.ipynb`

**Dataset Setup:**
1. Go to kaggle.com → Search "House Prices Advanced Regression Techniques"
2. Download train.csv
3. Place in same folder as notebook

**Key Results:**
- Typical MAE: $30,000-50,000 USD
- R² Score: 0.75-0.85 (good model fit)
- OverallQual (Quality rating) is THE strongest price predictor

**Run Time:** ~3 minutes

---

## Installation & Dependencies

### Python Version
Python 3.8+ recommended

### Core Dependencies
```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

### Task-Specific Dependencies
```bash
pip install yfinance requests transformers datasets torch accelerate
```

---

## Project Structure

```
DevelopersHub_AIML_Internship/
├── README.md
├── 1_Dataset_Visualization.ipynb
├── 2_Stock_Prediction.ipynb
├── 3_Heart_Disease.ipynb
├── 4_Health_Chatbot.ipynb
├── 5_Mental_Health_Chatbot.ipynb
└── 6_House_Price.ipynb
```

---

## Key Concepts Mastered

✅ Data visualization and exploratory analysis  
✅ Regression (predicting continuous values)  
✅ Classification (binary prediction)  
✅ Prompt engineering for safe AI  
✅ Fine-tuning language models  
✅ Machine learning evaluation metrics  
✅ Feature engineering  
✅ Real-world applications  

---

## Common Issues & Solutions

| Error | Solution |
|-------|----------|
| `ModuleNotFoundError` | Run: `pip install pandas` |
| `FileNotFoundError: heart.csv` | Download from Kaggle; place in correct folder |
| `HuggingFace API Error 401` | Generate new token from huggingface.co/settings/tokens |
| `CUDA out of memory` | Use Google Colab for Task 5 |
