# 📊 Credit Card Fraud Detection  

## 🎯 Project Overview  
This project uses **machine learning models** to detect fraudulent credit card transactions.  
The dataset is highly **imbalanced**, so techniques like **class weighting & feature engineering** were applied to improve fraud detection.  

## 📂 Dataset  
The dataset contains credit card transaction details, including:  
✔ `trans_date_trans_time` (Transaction timestamp)  
✔ `cc_num` (Credit card number)  
✔ `merchant`, `category` (Where the transaction occurred)  
✔ `amt` (Transaction amount)  
✔ `city`, `state`, `zip` (Location details)  
✔ `is_fraud` (**Target variable**: 1 = Fraud, 0 = Legitimate)  

📌 **Fraud cases are only ~0.5% of total transactions**, making detection challenging.  

## 🏗️ Machine Learning Models Used  
✅ **Random Forest (Best Model)** → Achieved **99.82% accuracy** with **0.60 recall** for fraud cases  
✅ **LSTM (Deep Learning Model)** → Tested, but didn’t improve recall significantly  
✅ **Feature Engineering** → Extracted **hour, day, month, and year** from timestamps  

## 📈 Results  
| Model         | Accuracy | Precision (Fraud) | Recall (Fraud) | F1-Score |
|--------------|----------|-------------------|----------------|----------|
| Random Forest | **99.82%** | **0.91** | **0.60** | **0.72** |
| LSTM | 99.70% | 0.50 | 0.56 | 0.53 |

## 🚀 How to Run the Project  
 **Clone the repository:**  
   ```bash
   git clone https://github.com/yourusername/credit-card-fraud-detection.git
   cd credit-card-fraud-detection
