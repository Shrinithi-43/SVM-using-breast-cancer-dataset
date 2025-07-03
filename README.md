## Support Vector Machines (SVM)

## 📌 Objective
The goal of this task is to implement **Support Vector Machines** (SVM) for binary classification using both **Linear** and **RBF kernels**, tune hyperparameters, and evaluate performance using cross-validation.

---

## 📁 Dataset
- **Breast Cancer Dataset** from [scikit-learn](https://scikit-learn.org/stable/modules/generated/sklearn.datasets.load_breast_cancer.html) was used.
- It contains features of cell nuclei from breast mass digitized images.
- Target: Malignant (0) or Benign (1).

---

## 🔧 Tools & Libraries Used
- Python
- NumPy
- Pandas
- Matplotlib
- Scikit-learn

---

## ⚙️ Steps Performed

### 1. **Data Loading and Preprocessing**
- Loaded dataset using `sklearn.datasets.load_breast_cancer`.
- Split into training and test sets.
- Standardized features using `StandardScaler`.

### 2. **Model Training**
- Trained **SVM with Linear Kernel**.
- Trained **SVM with RBF Kernel**.

### 3. **Evaluation**
- Used `accuracy_score` and `classification_report` to evaluate models.
- Observed performance difference between linear and non-linear kernels.

### 4. **Hyperparameter Tuning**
- Applied `GridSearchCV` on RBF SVM to tune `C` and `gamma`.
- Performed 5-fold cross-validation.

### 5. **(Optional)** Visualized decision boundaries using 2D synthetic dataset (`make_moons`).

---

## 📊 Results

| Model            | Accuracy |
|------------------|----------|
| SVM (Linear)     | ~96%     |
| SVM (RBF)        | ~98%     |
| RBF + GridSearch | ~99%     |

> Exact accuracy may vary depending on the random state.

---




