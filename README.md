# 📊 Credit Card Fraud Detection  

## 🎯 Project Overview  
This project uses **machine learning models** to detect fraudulent credit card transactions.  
The dataset is highly **imbalanced**, so techniques like **class weighting & feature engineering** were applied to improve fraud detection.  

## 📂 Dataset  

### 📥 Download the Dataset  
The dataset is too large to upload to GitHub. You can download it from Kaggle using the following link:  
🔗 [Credit Card Fraud Detection Dataset](https://www.kaggle.com/datasets/kartik2112/fraud-detection)

After downloading, place the CSV files in the project folder and update the file paths accordingly. 

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
✅ **Feature Engineering** → Extracted **hour, day, month, and year** from timestamps  

## 📈 Results  
| Model         | Accuracy | Precision (Fraud) | Recall (Fraud) | F1-Score |
|--------------|----------|-------------------|----------------|----------|
| Random Forest | **99.82%** | **0.91** | **0.60** | **0.72** |

## 🚀 How to Run the Project  
 **Clone the repository:**  
   ```bash
   https://github.com/PIYUSH-BAMNIA-25/credit-card-fraud-detection
   cd credit-card-fraud-detection
 ```
 **Install Dependencies**
 ```bash
pip install -r requirements.txt
```
**Run the Jupyter Notebook**
- Open Credit Card Fraud Detection.ipynb in Google Colab or Jupyter Notebook.

## Future Improvements
- 🔹 Deploy the model → Create an API for real-time fraud detection
