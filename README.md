# ❤️ Cardiovascular Risk Prediction - Machine Learning Project

![CHD_project_image](https://github.com/user-attachments/assets/6be7740c-5379-487d-9995-078a0ee845be)

## 📌 Project Type  

**Supervised Classification (Machine Learning)**  

**Contribution:** Individual Capstone Project  

**Author:** Ankesh Aman  

---

## 🧠 Problem Statement

This project leverages patient health data to predict the **10-year risk of developing coronary heart disease (CHD)** using supervised machine learning techniques. The dataset is sourced from an ongoing cardiovascular study of residents from **Framingham, Massachusetts**, containing over 4,000 records and 15 attributes.

The ultimate goal is to develop a model that can accurately flag individuals at risk for CHD, enabling earlier medical intervention and preventative care.

---

## 🗂 Data Description

Each attribute in the dataset represents a potential **risk factor**, grouped into the following categories:

### 🧍 Demographic:
- `Sex`: Male or Female
- `Age`: Age in years

### 🚬 Behavioral:
- `is_smoking`: Currently smoking (Yes/No)
- `Cigs Per Day`: Average daily cigarette consumption

### 🏥 Medical History:
- `BP Meds`: On blood pressure medication (Yes/No)
- `Prevalent Stroke`: History of stroke (Yes/No)
- `Prevalent Hyp`: History of hypertension (Yes/No)
- `Diabetes`: Diabetes status (Yes/No)

### 🧪 Current Medical Measurements:
- `Tot Chol`: Total cholesterol
- `Sys BP`: Systolic blood pressure
- `Dia BP`: Diastolic blood pressure
- `BMI`: Body Mass Index
- `Heart Rate`: Heart rate
- `Glucose`: Glucose level

### 🎯 Target Variable:
- `TenYearCHD`: Risk of developing CHD in 10 years (1 = Yes, 0 = No)

---

## 🧹 Data Cleaning & Preprocessing

To ensure high-quality model training, several preprocessing steps were carried out:

- **Missing Value Handling:** Imputed null values using strategies such as mean/median imputation and context-based decision-making.
- **Encoding:** Converted categorical variables into numeric representations using label encoding and one-hot encoding.
- **Outlier Detection & Treatment:** Used visual methods like boxplots and statistical methods (IQR) to identify and address outliers in variables like `BMI`, `Glucose`, and `Cigs Per Day`.
- **Feature Scaling:** Applied normalization using StandardScaler to bring all numerical features to a comparable scale.
- **Class Imbalance:** Addressed imbalanced classes using SMOTE (Synthetic Minority Oversampling Technique) to balance the target variable.

---

## 📊 Model Building & Evaluation

Multiple machine learning models were built and evaluated to identify the best-performing algorithm:

| Model               | Train Accuracy | Test Accuracy | Precision | Recall | F1 Score | AUC    |
|---------------------|----------------|----------------|-----------|--------|----------|--------|
| Logistic Regression | 68.71%         | 66.67%         | 65.90%    | 65.90% | 65.90%   | 73.18% |
| Decision Trees      | 73.40%         | 70.49%         | 66.77%    | 78.86% | 72.31%   | 77.78% |
| Random Forest       | 75.68%         | 71.53%         | 69.29%    | 74.96% | 72.01%   | 81.06% |
| XGBoost             | 93.38%         | 86.72%         | 88.10%    | 84.19% | 86.10%   | 93.25% |
| SVM                 | 99.91%         | 92.36%         | 91.59%    | 92.90% | 92.24%   | 97.37% |

> 📌 *Evaluation metrics like confusion matrix, ROC-AUC score, and classification report were used to assess model performance.*

---

## 🛠 Tools & Technologies Used

| Tool / Library       | Description                             |
|----------------------|-----------------------------------------|
| Python               | Core programming language               |
| Pandas & NumPy       | Data manipulation & numerical operations|
| Matplotlib & Seaborn | Data visualization                      |
| Scikit-learn         | Machine learning modeling & evaluation  |
| Imbalanced-learn     | Handling imbalanced datasets (SMOTE)    |
| Jupyter Notebook     | Interactive development environment     |

---
---

## 🧾 Conclusion

This project successfully explores the prediction of **10-year cardiovascular risk** using a range of supervised machine learning algorithms. Through detailed data analysis and modeling, several key clinical and demographic factors were identified as strong predictors of coronary heart disease (CHD).

**Key takeaways:**

- **Health Indicators Matter**: Features like **hypertension**, **diabetes**, **stroke history**, and **blood pressure medication usage** are clearly associated with a higher risk of CHD.
- **Lifestyle Risk Factors**: Interestingly, smoking status showed a nearly equal distribution among CHD-positive and CHD-negative individuals, suggesting that while smoking is a known risk factor, its impact may be influenced by other variables in this cohort.
- **Demographic Patterns**: The **median patient age is 49**, and **males show a slightly higher risk** of CHD compared to females.
- **Imbalanced Dataset**: A large number of patients do not have CHD, creating a class imbalance issue that was effectively addressed using **SMOTE (Synthetic Minority Oversampling Technique)**.

**From a modeling perspective:
**
- **Support Vector Machine (SVM)** with the radial kernel emerged as the **best-performing model**, achieving the highest **F1-score and AUC**, indicating strong balance between **precision and recall** and a high true positive rate.
- **XGBoost** also performed robustly, offering high test accuracy and strong generalization.
- **Data Scaling Impact**: Scaling affected model performance; notably, **SVM performed best without scaling**, highlighting the importance of preprocessing decisions.
- **SMOTE proved essential** for enhancing model sensitivity, especially in dealing with the imbalanced target variable.

### 💡 Final Thoughts

In healthcare-related machine learning tasks like CHD prediction, it's crucial to maintain a **balance between recall and precision**, as both false positives and false negatives can have serious implications. By aiming for a high **F1-score**, this project prioritizes a **balanced approach** that minimizes both kinds of errors.

With **more data**, particularly from the minority (CHD-positive) class, the models could be further improved for real-world deployment.

This project demonstrates the potential of machine learning to assist in early risk prediction, empowering healthcare professionals to take **proactive and preventative measures** for at-risk individuals.

---

## 🚀 How to Run This Project

1. **Clone the Repository**
   ```
   git clone https://github.com/yourusername/Cardiovascular-Risk-Prediction.git
   ```
2. **Navigate to the Project Directory**
  ```
  cd Cardiovascular-Risk-Prediction
  ```

3. **Launch Jupyter Notebook**

  ```
  jupyter notebook Cardiovascular_Risk_Prediction_Ankesh_Aman.ipynb
  ```
4. Run the Notebook Cells Follow along the notebook to see the full analysis, visualizations, and model results.

---
## 🙌 Acknowledgements

* Dataset courtesy of the Framingham Heart Study.

* Project completed as part of Capstone Project to demonstrate machine learning proficiency in healthcare applications

---






