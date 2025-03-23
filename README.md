# 📊 Credit Card Fraud Detection  

## 🎯 Project Overview

### 📌 Task Objectives
This project aims to develop a **fraud detection system** using machine learning techniques to distinguish fraudulent transactions from legitimate ones. The key objectives include:
- **Preprocessing financial transaction data** to extract meaningful insights.
- **Building a machine learning model** that accurately detects fraud.
- **Providing a clear and structured approach** to implementing and running the project.  
This project uses **machine learning models** to detect fraudulent credit card transactions.  

## 📂 Dataset

### 📥 Download the Dataset
The dataset is too large to upload to GitHub. You can download it from Kaggle using the following link:
🔗 [Credit Card Fraud Detection Dataset](https://www.kaggle.com/datasets/kartik2112/fraud-detection)

After downloading, place the CSV files in the project folder and update the file paths accordingly.
  
The dataset contains credit card transaction details, including:  
- ✔ `trans_date_trans_time` (*Transaction timestamp*)  
- ✔ `cc_num` (*Credit card number*)  
- ✔ `merchant`, `category` (*Where the transaction occurred*)  
- ✔ `amt` (*Transaction amount*)  
- ✔ `city`, `state`, `zip` (*Location details*)  
- ✔ `is_fraud` (**Target variable**: *1 = Fraud, 0 = Legitimate*)  

> 📌 **Fraud cases are only ~0.5% of total transactions**, making detection challenging.  

## 🏗️ Machine Learning Models Used  
- ✅ **Random Forest (Best Model)** → *Achieved **99.82% accuracy** with **0.60 recall** for fraud cases*  
- ✅ **Feature Engineering** → *Extracted **hour, day, month, and year** from timestamps*  

## 📈 Results  
| **Model**        | **Accuracy** | **Precision (Fraud)** | **Recall (Fraud)** | **F1-Score** |
|-----------------|------------|-------------------|----------------|----------|
| **Random Forest** | **99.82%**  | **0.91**          | **0.60**        | **0.72** |

## 🚀 How to Run the Project

### 📥 Download the Dataset
The dataset is too large to be included in the repository. You can download it from Kaggle:
🔗 [Credit Card Fraud Detection Dataset](https://www.kaggle.com/datasets/kartik2112/fraud-detection)

**Steps to use the dataset:**
1. Download Both CSV files (`fraudTrain.csv` or `fraudTest.csv`) from Kaggle.
2. Place them in the **project folder**.
3. Open the Jupyter Notebook (`Credit Card Fraud Detection.ipynb`).
4. Update file paths if necessary before running the notebook.

### 🛠️ Running the Project
**Clone the repository:**  
```bash
https://github.com/PIYUSH-BAMNIA-25/credit-card-fraud-detection
cd credit-card-fraud-detection
```

**Install Dependencies:**  
```bash
pip install -r requirements.txt
```

**Run the Jupyter Notebook:**  
- Open `Credit Card Fraud Detection.ipynb` in **Google Colab** or Jupyter Notebook.
- Ensure the dataset is correctly placed before executing the notebook.

### 💾 Model File
Due to size limitations, the trained model file (`credit_fraud_model.pkl`) is not uploaded to GitHub.
- **Option 1:** Train the model yourself using the notebook.
- **Option 2:** Download the pre-trained model from Google Drive:
  🔗 [Download Model](https://drive.google.com/file/d/1VcuzpwXDWcZdNRdwULXM0Yf6kfhinw-P/view?usp=sharing)  


## 💡 Future Improvements  
- 🔹 **Use XGBoost** → *Further optimize fraud detection*  
- 🔹 **Deploy the model** → *Create an **API for real-time fraud detection***    

