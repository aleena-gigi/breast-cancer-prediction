# 🧬 Breast Cancer Survival Prediction using METABRIC Dataset

This academic project uses machine learning to classify the **overall survival** of breast cancer patients using **clinical** and **mRNA gene expression data** from the METABRIC dataset.

---

## 📁 Dataset Description

The METABRIC dataset includes:

- **Clinical features**: age, tumor stage, therapy types, receptor statuses, etc.
- **Genetic features**:
  - **mRNA expression Z-scores** for 331 genes
  - **Mutation indicators** for 175 genes

**Target variable**: `overall_survival` (1 = Living, 0 = Died)

Dataset Source: https://www.kaggle.com/datasets/raghadalharbi/breast-cancer-gene-expression-profiles-metabric

---

## 📊 Project Workflow

1. **Data Loading**
   - Dataset read using `pandas`
   - Target column mapped to binary labels

2. **Data Cleaning**
   - Handled missing values (mean imputation for numerical)
   - Dropped all-NaN columns
   - Converted object types

3. **Feature Encoding**
   - `One-Hot Encoding` for categorical columns

4. **Feature Scaling**
   - Standardized all numerical features using `StandardScaler`

5. **Principal Component Analysis**
   - High dimensional gene mRNA expression data converted to 10 PCs'
6. **Train-Test Split**
   - Data split into 80% train / 20% test

7. **Modeling** *(Coming in next steps)*
   - Multiple ML algorithms to be tested: Logistic Regression, Random Forest, XGBoost, etc.
   - Model comparison using accuracy, F1 score, ROC-AUC

---

## ⚙️ How to Run

1. Clone the repo:
   ```bash
   git clone https://github.com/aleena-gigi/breast-cancer-prediction
   cd breast-cancer-prediction ```

2. Install Dependencies:
   ```pip install -r requirements.txt ```

3. References:
   ```METABRIC Dataset: Available publicly for research purposes(https://www.kaggle.com/datasets/raghadalharbi/breast-cancer-gene-expression-profiles-metabric) ```

4. Authors:
   Aleena Gigi
   Tirthankar Sen
   Rajendra Warke
   
## 🎓 Academic Project

This project was completed as part of the coursework for **AAI-501** in April 2025.
- **Group No.**: 5  
- **Team Members**: 3 students  
- **Semester**: March 2025
- **Course**: AAI-501 (Introduction to Artificial Intelligence)