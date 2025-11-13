# 🩺 AI-Driven Heart Disease Prediction

This project applies various **machine learning algorithms** to predict the likelihood of heart disease in patients.  
Developed as part of the **MSc Artificial Intelligence (Introduction to AI module)** at Berlin School of Bussiness and Innovation.



# 🚀 Project Overview

Cardiovascular diseases are one of the leading causes of death globally.  
This project explores how **AI and ML models** can assist in early detection by identifying hidden data patterns that may not be visible through manual diagnosis.

Five models were trained and evaluated:
- Logistic Regression  
- Decision Tree  
- Random Forest  
- Gradient Boosting  
- Support Vector Machine (SVM)

---

## 🧩 Dataset

The dataset contains patient medical attributes such as:
- Age, Sex, Chest Pain Type, Blood Pressure, Cholesterol, etc.  
- Target variable: `1` = Heart Disease Present, `0` = No Heart Disease

> Source: [UCI Heart Disease Dataset](https://archive.ics.uci.edu/ml/datasets/heart+disease)  
> Data preprocessing handled missing values, outliers, and feature scaling using **StandardScaler**.

---

## ⚙️ Preprocessing Steps

1. **Handle Missing Values** – Replace or impute missing entries.  
2. **Feature Scaling** – Standardized numerical features using `StandardScaler`.  
3. **Outlier Handling** – Managed using IQR method and median imputation.  
4. **Feature Correlation** – Heatmap used for correlation visualization and redundancy reduction.  
5. **Data Balancing** – Checked target class balance for model fairness.

---

## 🤖 Model Training

| Classifier | Accuracy | Precision | Recall | F1-score | AUC-ROC |
|-------------|-----------|------------|---------|-----------|----------|
| Logistic Regression | 0.8361 | 0.8214 | 0.8214 | 0.8214 | 0.942 |
| Decision Tree | 0.6885 | 0.6800 | 0.6071 | 0.6415 | 0.682 |
| Random Forest | 0.8852 | 0.8387 | 0.9286 | 0.8814 | 0.951 |
| Gradient Boosting | 0.8852 | 0.8327 | 0.9286 | 0.8814 | 0.951 |
| SVM | 0.8361 | 0.8462 | 0.7857 | 0.8148 | 0.937 |

> The **Gradient Boosting Classifier** achieved the best AUC-ROC score (0.9513).

---

## 📈 Visualizations

- ROC Curves for each classifier  
- Confusion Matrices comparing true/false predictions  
- Feature Correlation Heatmap  

---

## 🧠 Insights

- **Ensemble models (Random Forest, Gradient Boosting)** outperformed individual classifiers.  
- **Decision Tree** suffered from overfitting.  
- **SVM and Logistic Regression** performed consistently well but less than ensemble methods.

---

## 💡 Future Improvements

- Apply **deep learning** architectures for feature extraction.  
- Integrate **hyperparameter optimization**.  
- Develop an **explainable AI interface** for clinical decision support.

---

## 🧰 Tech Stack

- Python  
- Scikit-learn  
- Pandas, NumPy  
- Matplotlib, Seaborn  
- Google Colab

---

## 📎 Resources

- 📘 Full Report: [Gaurav_AI_Practical_Report.pdf](./reports/Gaurav_AI_Practical_Report.pdf)
- 📓 Notebook: [Colab Link](https://colab.research.google.com/drive/1CMVKuUmO2Yituo2V-ECKm0HnjRnLtm2v?usp=sharing)

---

## 👨‍💻 Author

**Gaurav Arun**  
MSc Artificial Intelligence, 2025  
Berlin, Germany  

---

## ⚖️ License
This project is licensed under the MIT License – see the [LICENSE](./LICENSE) file for details.
