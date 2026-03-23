# Credit Card Fraud Detection

## Problem
Credit card fraud detection is a classic imbalanced 
classification problem — only 0.23% of transactions 
are fraudulent.

## Dataset
- 87,239 real banking transactions
- 30 features (V1-V28 PCA + Time + Amount)
- Target : Class (0 = Normal, 1 = Fraud)

## Approach
1. Data Cleaning
2. Class Imbalance Analysis (0.23% fraud rate)
3. SMOTE to balance training data
4. 3 Models compared : Random Forest, XGBoost, LightGBM
5. Evaluation : Recall + ROC-AUC
6. Feature Importance Analysis

## Results

| Model | Precision | Recall | F1 | ROC-AUC |
|-------|-----------|--------|----|---------|
| **Random Forest** | **0.89** | **0.95** | **0.92** | 0.9996 |
| XGBoost | 0.86 | 0.93 | 0.89 | 0.9994 |
| LightGBM | 0.85 | 0.95 | 0.90 | 0.9998 |

Best model : **Random Forest**
- 39 frauds detected out of 41
- Only 2 missed frauds
- 5 false alarms

## Technologies
Python, Pandas, NumPy, Scikit-learn, XGBoost, LightGBM, SMOTE, Matplotlib, Seaborn

## Files
- `fraud_detection.ipynb` — Main notebook
- `creditcard.csv` — Dataset

##  Author
— Data Scientist | Open to Remote Work Worldwide
