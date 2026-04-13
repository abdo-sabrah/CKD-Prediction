# Kidney Disease Classification Project

This project applies **machine learning models** to classify patients based on clinical features related to kidney health.  
The dataset (`new_model.csv`) contains 400 records with 14 medical attributes such as blood pressure, albumin, sugar, red blood cell count, hemoglobin, and hypertension status.

---

## 📊 Dataset Overview
- **Rows:** 400  
- **Columns:** 14 features + target (`Class`)  
- **Target:** `Class` (1 = affected, 0 = not affected)  
- **No missing values** after preprocessing  
- Outliers handled (e.g., removed abnormal sodium values)

**Key Features:**
- `Bp`: Blood Pressure  
- `Sg`: Specific Gravity  
- `Al`: Albumin  
- `Su`: Sugar  
- `Rbc`: Red Blood Cell  
- `Bu`: Blood Urea  
- `Sc`: Serum Creatinine  
- `Sod`: Sodium  
- `Pot`: Potassium  
- `Hemo`: Hemoglobin  
- `Wbcc`: White Blood Cell Count  
- `Rbcc`: Red Blood Cell Count  
- `Htn`: Hypertension  

---

## 🔍 Exploratory Data Analysis (EDA)
- **Histograms & scatterplots** to visualize distributions and relationships.  
- **Correlation heatmap** to identify feature importance.  
- **Class balance check** using `sns.countplot`.  
- Investigated abnormal values (e.g., sodium = 4.5, creatinine > 76).  

---

## ⚙️ Models Used
Five classifiers were trained and evaluated:
- Logistic Regression  
- Decision Tree  
- Random Forest  
- K‑Nearest Neighbors (KNN)  
- Support Vector Machine (SVM)  

### Cross‑Validation Scores
| Model                  | CV Score |
|-------------------------|----------|
| Logistic Regression     | 0.979    |
| Decision Tree           | 0.971    |
| Random Forest           | 0.991    |
| KNN                     | 0.982    |
| SVM                     | 0.988    |

### Test Accuracy
| Model                  | Accuracy |
|-------------------------|----------|
| Logistic Regression     | 0.983    |
| Decision Tree           | 0.950    |
| Random Forest           | 0.967    |
| KNN                     | 0.983    |
| SVM                     | 0.983    |

---

## 📈 Results
- **Best performing models:** Logistic Regression, KNN, and SVM (≈98% accuracy).  
- Confusion matrices and classification reports confirm strong precision and recall for both classes.  
- Random Forest also performed well but slightly lower than the top models.

---

## 🛠️ Tech Stack
- Python (Pandas, NumPy, Scikit‑learn, Seaborn, Matplotlib, Plotly)  
- Jupyter Notebook for experimentation  
- Machine Learning algorithms for classification  

---

## 🚀 How to Run
1. Clone the repo:
   ```bash
   git clone https://github.com/yourusername/kidney-disease-classification.git
