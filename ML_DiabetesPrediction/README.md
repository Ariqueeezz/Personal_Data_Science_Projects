# 🏥 End-to-End Diabetes Prediction System

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Scikit-Learn](https://img.shields.io/badge/scikit--learn-%23F7931E.svg?style=for-the-badge&logo=scikit-learn&logoColor=white)
![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white)
![Imbalanced-Learn](https://img.shields.io/badge/Imbalanced--Learn-SMOTE-blue?style=for-the-badge)
![GoogleColab](https://img.shields.io/badge/Made%20with-Colab-orange?style=for-the-badge&logo=GoogleColab)

> **"Early detection allows for early intervention."**
>> This project focuses on building a robust Machine Learning pipeline to predict diabetes likelihood based on health indicators. It demonstrates a complete lifecycle from **Exploratory Data Analysis (EDA)** to **Model Engineering** and finally **Production Readiness**.

---

## 📌 Project Architecture

The development process is structured into three distinct phases to ensure scalability and reproducibility.

```text
📂 Diabetes_Prediction_Project/
│
├── 📓 1. Experiment_DiabetesPrediction.ipynb   # Phase 1: Discovery & Baseline
├── 📓 2. Experiment2_DiabetesPrediction.ipynb  # Phase 2: Engineering & Optimization
├── 📓 3. Production_DiabetesPrediction.ipynb   # Phase 3: Final Pipeline & Serialization
├── 📄 diabetes_binary_health_indicators.csv    # Dataset (Source: BRFSS 2015)
└── 📄 README.md                                # Project Documentation
```

## 🔍 Phase 1: Discovery (Experiment 1)
**Goal**: Understand the data landscape and establish a baseline performance.

- **Key Finding**: The dataset is heavily imbalanced (86% Non-Diabetes vs 14% Diabetes).
- **Action**: Conducted Correlation Analysis to identify key features (e.g., HighBP, HighChol, BMI).
- **Baseline Models**: Tested Decision Tree, KNN, and Naive Bayes.
- **Metric Focus**: Prioritized Recall over Accuracy, as minimizing False Negatives (missed diagnoses) is critical in medical fields.

## ⚙️ Phase 2: Engineering & Optimization (Experiment 2)
**Goal**: Solve the imbalance problem and maximize model performance using advanced techniques.

We conducted a comparative study of 4 scenarios using **Random Forest** and **XGBoost**:

- Base Model (No treatment).
- **Data-Level Optimization**: Using SMOTEENN (Hybrid Sampling: SMOTE + Edited Nearest Neighbours).
- **Algorithm-Level Optimization**: Hyperparameter tuning using GridSearchCV.
- **Hybrid Approach**: Combining SMOTEENN + GridSearchCV.

### 💡 Key Insight (The "Golden Rule")
>*"Data-Level Optimization (Resampling) significantly outperformed Algorithm-Level Optimization (Tuning). Tuning parameters on imbalanced data yields minimal improvement compared to balancing the data first.*

**Best Result**:
- **Technique**: Random Forest Classifier + SMOTEENN.
- **Performance**: Successfully improved the model's ability to detect positive cases (Diabetes) while maintaining stability.

## 🚀 Phase 3: Production
**Goal**: Prepare the final model for deployment.

In this notebook, we moved from "Research" to "Engineering":

- **Pipeline Construction**: Consolidated the best preprocessing and modeling steps.
- **Retraining**: Trained the final model on the full dataset.
- **Sanity Check**: Validated that the trained model performs as expected on sample data.
- **Serialization**: Exported the model (Pickle/Joblib) for integration with web apps.

## 🛠️ Tech Stack & Tools
| Category | Tools Used |
|---|---|
| **Language** | Python 3.9+ |
| **Data Manipulation** | Pandas, NumPy |
| **Visualization** | Matplotlib, Seaborn |
| **Machine Learning** | Scikit-Learn, XGBoost | 
| **Imbalance Handling** | Imbalanced-Learn (SMOTEENN) |
| **Environment** | Jupyter Notebook / Google Colab |

