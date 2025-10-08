# 🫁 Lung Cancer Prediction using SVM

## 📄 Project Overview  
This project focuses on predicting **lung cancer** using a dataset of various lifestyle and health-related factors.  
It employs a **Support Vector Machine (SVM)** classifier to analyze and predict whether an individual is likely to have lung cancer based on given attributes.  

---

## 📊 Dataset Description  
The dataset used is **`survey lung cancer.csv`** containing **309 samples** and **16 features**.  

### 🧬 Features  
- **GENDER** 🧑‍🤝‍🧑  
- **AGE** 🎂  
- **SMOKING** 🚬  
- **YELLOW_FINGERS** ☝️  
- **ANXIETY** 😰  
- **PEER_PRESSURE** 🧍‍♂️  
- **CHRONIC DISEASE** 🩺  
- **FATIGUE** 😴  
- **ALLERGY** 🤧  
- **WHEEZING** 😮‍💨  
- **ALCOHOL CONSUMING** 🍺  
- **COUGHING** 🤧  
- **SHORTNESS OF BREATH** 😤  
- **SWALLOWING DIFFICULTY** 🍽️  
- **CHEST PAIN** 💔  
- **LUNG_CANCER** (Target Variable)

---

## 🧠 Model Workflow  

### 1️⃣ Data Preprocessing  
- Checked for missing values ✅  
- Encoded categorical variables using **LabelEncoder**  
- Standardized data with **StandardScaler**

### 2️⃣ Train-Test Split  
- Training data: 80%  
- Test data: 20%

### 3️⃣ Model Training  
- Algorithm: **Support Vector Classifier (SVC)**  
- Library: `scikit-learn`

```python
from sklearn.svm import SVC
model = SVC()
model.fit(x_train, y_train)
| Metric    | Class 0 | Class 1 |
| --------- | ------- | ------- |
| Precision | 0.25    | 0.98    |
| Recall    | 0.50    | 0.95    |
| F1-Score  | 0.33    | 0.97    |
sns.heatmap(cm, annot=True, fmt='g')
plt.title('Confusion Matrix')
sns.heatmap(cm, annot=True, fmt='g')
plt.title('Confusion Matrix')
sns.heatmap(cm, annot=True, fmt='g')
plt.title('Confusion Matrix')
Results Summary

✅ High accuracy (93.5%) on test data
✅ SVM model effectively distinguishes between lung cancer cases
⚠️ Slight imbalance between classes observed
Future Improvements

Implement feature selection

Try ensemble models (Random Forest, XGBoost)

Optimize SVM hyperparameters using GridSearchCV

👨‍💻 Author

Project by: [amrita kumari]
🗓️ Date: 8October 2025
📍 Tool Used: Google Colab
