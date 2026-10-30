# Breast Cancer Diagnosis Classification
**Course:** Introduction to Data Science (Intdsci) – Final Project  
**Institution:** De La Salle Lipa, College of Information Technology and Engineering, Computer Science Department  

---

## 📌 Project Overview
This project performs supervised binary classification to predict whether a breast mass is **Malignant (M)** or **Benign (B)** using digitised measurements of fine-needle aspirate (FNA) cell nuclei.

The dataset is the **Wisconsin Diagnostic Breast Cancer (WDBC)** dataset (Wolberg, Street, & Mangasarian, 1995) from the UCI Machine Learning Repository.

---

## 📂 Repository Contents
- [`breast_cancer_classification.ipynb`](breast_cancer_classification.ipynb): Complete end-to-end Jupyter Notebook with exploratory data analysis (EDA), preprocessing, scaling, baseline & machine learning model training, and comparative evaluation.
- [`breast_cancer.csv`](breast_cancer.csv): The raw Wisconsin Diagnostic Breast Cancer dataset (569 rows, 32 attributes).
- [`Breast_Cancer_Classification_Documentation(1).pdf`](Breast_Cancer_Classification_Documentation(1).pdf): Comprehensive documentation and report covering project methodology, analysis, and conclusions.

---

## 📊 Models & Comparative Evaluation
Models evaluated on an 80/20 stratified split (114 test samples):
1. **DummyClassifier Baseline** (majority class strategy)
2. **Logistic Regression** (linear model with StandardScaler)
3. **Random Forest Classifier** (non-linear ensemble)

### Test Set Performance Summary
| Model | TN (Benign) | FP | FN | TP (Malignant) |
| :--- | :---: | :---: | :---: | :---: |
| **Dummy Baseline** | 72 | 0 | 42 | 0 |
| **Logistic Regression** | **72** | **0** | **4** | **38** |
| **Random Forest** | 71 | 1 | 6 | 36 |

**Key Predictive Features:**
- `perimeter_worst`
- `concave points_worst`
- `radius_se`
- `texture_worst`

---

## 🚀 How to Run the Notebook
1. Clone the repository:
   ```bash
   git clone https://github.com/Zelo23/FInals_Introduction_To_Data_Science.git
   cd FInals_Introduction_To_Data_Science
   ```
2. Install required packages:
   ```bash
   pip install numpy pandas scikit-learn matplotlib seaborn jupyter
   ```
3. Open and run the notebook:
   ```bash
   jupyter notebook breast_cancer_classification.ipynb
   ```
