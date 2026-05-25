# 🩺 Diabetes Risk Prediction

A machine learning classification project that predicts whether a person is at risk of diabetes based on health parameters. Built using Python and Scikit-learn with a complete pipeline from data preprocessing to model evaluation.

---

## 📌 Problem Statement

Diabetes is one of the most prevalent chronic diseases globally. Early prediction of diabetes risk using patient health data can help in timely medical intervention. This project builds a classification model to predict whether a patient is diabetic or not based on diagnostic health measurements.

---

## 📊 Dataset

- **Source:** Pima Indians Diabetes Dataset (UCI Machine Learning Repository)
- **Target variable:** `Outcome` — 1 (Diabetic) / 0 (Non-Diabetic)
- **Features include:**
  - `Pregnancies` — number of pregnancies
  - `Glucose` — plasma glucose concentration
  - `BloodPressure` — diastolic blood pressure (mm Hg)
  - `SkinThickness` — triceps skinfold thickness (mm)
  - `Insulin` — 2-hour serum insulin
  - `BMI` — body mass index
  - `DiabetesPedigreeFunction` — diabetes likelihood based on family history
  - `Age` — age of the patient

---

## ⚙️ Tech Stack

| Tool | Purpose |
|---|---|
| Python 3.x | Core programming language |
| Pandas | Data loading and manipulation |
| NumPy | Numerical operations |
| Scikit-learn | ML models, preprocessing, evaluation |
| Matplotlib | Data visualization |
| Seaborn | Statistical plots and heatmaps |

---

## 🔄 Project Workflow

```
Raw Data → EDA → Preprocessing → Model Training → Evaluation → Results
```

### 1. Exploratory Data Analysis (EDA)
- Checked class balance (diabetic vs non-diabetic)
- Plotted feature distributions and boxplots
- Correlation heatmap to identify important features

### 2. Data Preprocessing
- Replaced zero values in Glucose, BMI, Insulin with median (zeros are medically invalid)
- Applied feature scaling using `StandardScaler`
- Split data into 80% train / 20% test

### 3. Model Building
Trained and compared the following classification models:
- Logistic Regression
- Decision Tree Classifier
- Random Forest Classifier
- K-Nearest Neighbors (KNN)
- Support Vector Machine (SVM)

### 4. Evaluation Metrics
- **Accuracy**
- **Precision & Recall**
- **F1 Score**
- **Confusion Matrix**

---

## 📈 Results

| Model | Accuracy | Precision | Recall |
|---|---|---|---|
| Logistic Regression | ~77% | 0.74 | 0.72 |
| Decision Tree | ~72% | 0.68 | 0.70 |
| Random Forest | ~80% | 0.78 | 0.75 |
| SVM | ~79% | 0.76 | 0.74 |
| KNN | ~75% | 0.72 | 0.71 |

> ✅ **Best model: Random Forest Classifier** with ~80% accuracy

---

## 📂 Project Structure

```
diabetes-risk-prediction/
│
├── data/
│   └── diabetes.csv              # Raw dataset
│
├── notebooks/
│   └── diabetes_prediction.ipynb # Main Jupyter notebook
│
├── outputs/
│   └── plots/                    # EDA and result visualizations
│
├── requirements.txt              # Python dependencies
└── README.md
```

---

## 🚀 How to Run

```bash
# 1. Clone the repository
git clone https://github.com/prathameshdeshpande-dv/diabetes-risk-prediction.git
cd diabetes-risk-prediction

# 2. Install dependencies
pip install -r requirements.txt

# 3. Open the notebook
jupyter notebook notebooks/diabetes_prediction.ipynb
```

---

## 📦 Requirements

```
pandas
numpy
scikit-learn
matplotlib
seaborn
jupyter
```

---

## 🔑 Key Learnings

- Glucose level and BMI are the strongest predictors of diabetes risk
- Replacing invalid zero values significantly improved model accuracy
- Random Forest outperformed all other models due to its ensemble nature
- Recall is more important than precision here — missing a diabetic patient is costlier than a false alarm

---

## 👤 Author

**Prathamesh Deshpande**
- 📧 pvdeshpande06@gmail.com
- 💼 [LinkedIn](https://www.linkedin.com/in/prathamesh-deshpande-227862275)
- 💻 [GitHub](https://github.com/prathameshdeshpande-dv)
