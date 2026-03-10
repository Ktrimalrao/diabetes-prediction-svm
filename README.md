# 🩺 Diabetes Prediction using Machine Learning (SVM)

## 📌 Project Overview
The **Diabetes Prediction System** is a Machine Learning based web application that predicts whether a person is diabetic or non-diabetic based on medical input parameters.  

The model is trained on the **Pima Indians Diabetes Dataset** and deployed using a **Flask web application**, allowing users to input health-related features and get instant predictions.

This project demonstrates the **complete ML pipeline**, including:
- Data preprocessing
- Exploratory Data Analysis (EDA)
- Model training
- Model serialization using Pickle
- Web deployment using Flask

---

## 🎯 Problem Statement
Diabetes is a common chronic disease that requires early diagnosis and monitoring. Predicting diabetes using medical parameters can help in early detection and preventive healthcare.

The goal of this project is to build a **Machine Learning model that predicts the likelihood of diabetes** based on patient medical attributes.

---

## 📊 Dataset Description
The dataset used in this project is the **Pima Indians Diabetes Dataset**.

### Features

| Feature | Description |
|------|-------------|
| Pregnancies | Number of pregnancies |
| Glucose | Plasma glucose concentration |
| BloodPressure | Diastolic blood pressure (mm Hg) |
| SkinThickness | Triceps skin fold thickness |
| Insulin | 2-Hour serum insulin |
| BMI | Body Mass Index |
| DiabetesPedigreeFunction | Diabetes pedigree function |
| Age | Age of the patient |
| Outcome | Target variable (1 = Diabetic, 0 = Non-Diabetic) |

Example Data:

| Pregnancies | Glucose | BloodPressure | SkinThickness | Insulin | BMI | DiabetesPedigreeFunction | Age | Outcome |
|-------------|--------|---------------|---------------|--------|-----|---------------------------|-----|--------|
| 6 | 148 | 72 | 35 | 0 | 33.6 | 0.627 | 50 | 1 |
| 1 | 85 | 66 | 29 | 0 | 26.6 | 0.351 | 31 | 0 |

---

## ⚙️ Project Workflow

### 1️⃣ Data Analysis
Exploratory Data Analysis was performed to understand:
- Feature distribution
- Correlation between variables
- Data imbalance
- Outliers

### 2️⃣ Data Preprocessing
Steps performed:
- Handling missing values
- Feature scaling using **StandardScaler**
- Feature selection

### 3️⃣ Model Training
Multiple machine learning models were experimented with, including:
- Logistic Regression
- Decision Tree
- Support Vector Machine (SVM)

The **Support Vector Machine (SVM)** model was selected for prediction.

### 4️⃣ Model Serialization
The trained model and scaler were saved using **Pickle**:


modelForPrediction.pkl
standardScalar.pkl


These files are loaded inside the Flask application for real-time predictions.

### 5️⃣ Web Application
A Flask web interface allows users to:
- Enter patient health parameters
- Submit data
- Receive diabetes prediction results instantly

---

## 🗂 Project Structure

```
diabetes-prediction-svm
│
├── Dataset
│ └── diabetes.csv
│
├── Model
│ ├── modelForPrediction.pkl
│ └── standardScalar.pkl
│
├── Notebook
│ ├── Decision_Tree_SVC.ipynb
│ └── Logistic_Regression.ipynb
│
├── templates
│ ├── index.html
│ └── home.html
│
├── application.py
├── requirements.txt
├── data.json
└── README.md
```



---

## 🧠 Model Input Features
The model requires the following input features:

1. Pregnancies
2. Glucose
3. BloodPressure
4. SkinThickness
5. Insulin
6. BMI
7. DiabetesPedigreeFunction
8. Age

---

## 🚀 Running the Project Locally

### 1️⃣ Clone the Repository

```bash
git clone [https://github.com/Ktrimalrao/diabetes-prediction-svm.git](https://github.com/Ktrimalrao/diabetes-prediction-svm.git)

```

### 2️⃣ Navigate to the Project Directory
```
cd diabetes-prediction-svm
```

### 3️⃣ Install Dependencies

```
pip install -r requirements.txt
```

### 4️⃣ Run the Flask Application
```
python application.py
```


### 5️⃣ Open in Browser
```
http://localhost:5000
```


## 📦 Requirements

- pandas
- numpy
- scikit-learn
- seaborn
- Flask

Install using:

```bash
pip install -r requirements.txt
```

## 🖥 Example Prediction Flow

1. User enters health data
2. Data is scaled using `StandardScaler`
3. Model predicts the outcome
4. Result displayed as:
      ```
        Diabetic
          or
        Non-Diabetic
      ```

   ## 📈 Technologies Used

- Python
- Flask
- Scikit-learn
- Pandas
- NumPy
- Seaborn
- Pickle

---

## 💡 Future Improvements

- Improve UI with better frontend design
- Add probability score for predictions
- Deploy the application on cloud platforms
- Add model monitoring
- Integrate with healthcare datasets


## 👨‍💻 Author

**K. Trimal Rao**

- 🎓 B.Tech in Computer Science and Engineering  
- 💻 Data Science | Machine Learning | AI

🔗 LinkedIn  
[https://www.linkedin.com/in/k-trimal-rao-397924253/](https://www.linkedin.com/in/k-trimal-rao-397924253/)

🔗 GitHub  
[https://github.com/Ktrimalrao](https://github.com/Ktrimalrao)

📧 Email  
[ktrimalrao16@gmail.com](mailto:ktrimalrao16@gmail.com)
