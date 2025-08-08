# 🏡 Boston Housing Price Prediction

An end-to-end **Data Science Regression Project** built to predict housing prices using machine learning and statistical modeling. This project covers the complete data science pipeline — from **EDA and preprocessing to model building, hyperparameter tuning, and evaluation** — using the well-known **Boston Housing Dataset**.

---

## 🚀 Project Highlights

✅ Hands-on implementation of both **Statistical Models** and **Machine Learning Algorithms**  
✅ Real-world **Data Preprocessing Techniques** including outlier detection using **LOF**  
✅ Thorough **Exploratory Data Analysis (EDA)**: Univariate, Bivariate, and Statistical Tests  
✅ Performed **Feature Engineering**, **Scaling**, and **Multicollinearity Check (VIF)**  
✅ Used **Grid Search CV** for Hyperparameter Tuning  
✅ Compared model performance using **MSE** and **R² Score**  
✅ Feature importance analysis from **Random Forest**

---

## 📂 Table of Contents

- [1. Dataset Overview](#1-dataset-overview)
- [2. Project Structure](#2-project-structure)
- [3. Step-by-Step Workflow](#3-step-by-step-workflow)
- [4. Tools and Libraries](#4-tools-and-libraries)
- [5. Results Summary](#5-results-summary)
- [6. Contact](#8-contact)

---

## 📊 1. Dataset Overview

The [Boston Housing Dataset](https://scikit-learn.org/stable/modules/generated/sklearn.datasets.load_boston.html) contains information collected by the U.S Census Service concerning housing in the area of Boston Mass.  

**Target Variable:** `MEDV` (Median value of owner-occupied homes in $1000s)  
**Features:** 14 numerical and categorical predictors like `RM` (rooms), `LSTAT` (lower status population %), `CRIM` (crime rate), etc.

---

## 🧱 2. Project Structure

```bash
1. Environment Setup and Data Overview
2. Univariate Analysis
3. Bivariate Analysis
4. Data Preprocessing
5. Model Training & Evaluation
```

---

## 🔍 3. Step-by-Step Workflow

### 📌 Step 1: Environment Setup & Data Overview
- Imported all essential libraries.
- Loaded the dataset and did initial data screening (`.info()`, `.describe()`, null check).

---

### 📌 Step 2: Univariate Analysis
- Visualized **distribution of features** and the **target** using histograms and boxplots.
- Calculated and interpreted **skewness** and **kurtosis** to understand the shape of the distributions.

---

### 📌 Step 3: Bivariate Analysis
- Created **scatter plots** between each numerical feature and the target variable to observe relationships.
- Generated **correlation heatmap** to identify strong and weak relationships.
- Performed **statistical significance tests**:
  - **Pearson correlation** for numerical vs numerical
  - **T-test** for binary categorical vs numerical

---

### 📌 Step 4: Data Preprocessing
- ✅ No missing values were found.
- 🔍 Detected **outliers** using **Local Outlier Factor (LOF)** and removed them.
- 🧪 Scaled features using **StandardScaler** for linear models.

---

### 📌 Step 5: Model Training & Evaluation

#### ✔️ StatsModels (OLS)
- Built a baseline regression model.
- Removed statistically insignificant variables.
- Checked **VIF values** to reduce multicollinearity.

#### ✔️ Scikit-learn Linear Regression
- Trained a model using scaled features.
- Applied **GridSearchCV** to explore hyperparameters.

#### ✔️ Random Forest Regressor
- Used **ensemble technique** to capture non-linearities.
- Tuned with **GridSearchCV**.
- Extracted **feature importances** for interpretation.

#### 📈 Evaluation Metrics
- Used **R² Score** and **Mean Squared Error (MSE)** for model comparison.
- Compared models on performance and interpretability.

---

## 🧰 4. Tools and Libraries

| Tool           | Purpose                          |
|----------------|----------------------------------|
| `Pandas`       | Data manipulation and wrangling |
| `NumPy`        | Numerical operations             |
| `Matplotlib`   | Data visualization               |
| `Seaborn`      | Statistical plots                |
| `Scikit-learn` | Machine learning models & tools  |
| `Statsmodels`  | Statistical modeling             |
| `SciPy`        | Hypothesis testing               |

---

## 🏁 5. Results Summary

| Model                   | R² Score | MSE     |
|------------------------|----------|----------|
| StatsModels OLS        | ~0.77    |   -      |
| Linear Regression (SKL)| ~0.78    | ~15.63   |
| Random Forest Regressor| ~0.86    | ~9.30    |

- 📌 `RM` (average number of rooms per dwelling) and `LSTAT` (lower status population %) were the most influential features.
- Random Forest gave the best performance, but the Linear model offers more interpretability.

---

## 📬 6. Contact

Made with ❤️ by **Mit Trivedi**  
📧 Email: trivedimit04@gmail.com  
🔗 [LinkedIn](www.linkedin.com/in/mit-trivedi-8714a5344) | [GitHub](https://github.com/trivedimit)

---

## ⭐ If you found this useful, give it a star and share it! ⭐
