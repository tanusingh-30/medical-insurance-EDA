# Medical Insurance Cost — Exploratory Data Analysis

An Exploratory Data Analysis project focused on understanding the factors associated with medical insurance charges using Python.

## 📌 Project Overview

Medical insurance costs can vary significantly between individuals. This project explores the relationships between insurance charges and different demographic, health-related, lifestyle, and regional factors.

The analysis focuses on identifying patterns in the dataset, understanding relationships between variables, performing statistical analysis, and preparing a cleaned and feature-engineered dataset for potential machine learning applications.

## 🎯 Objectives

* Understand the structure and characteristics of the insurance dataset
* Explore the distribution of numerical and categorical variables
* Identify factors associated with medical insurance charges
* Analyze relationships between age, BMI, smoking status, and insurance charges
* Perform data cleaning and preprocessing
* Apply feature engineering
* Analyze correlations between features and insurance charges
* Perform statistical testing for categorical features
* Prepare a final processed dataset for further machine learning analysis

## 🛠️ Technologies Used

* Python
* NumPy
* Pandas
* Matplotlib
* Seaborn
* SciPy
* Scikit-learn
* Jupyter Notebook

## 📊 Exploratory Analysis

The project explores:

* Distribution of age, BMI, number of children, and insurance charges
* Distribution of categorical variables such as sex, smoking status, and region
* Insurance charges across smokers and non-smokers
* Relationship between age and insurance charges
* Relationship between BMI and insurance charges
* Insurance charges across different regions
* Insurance charges across different sexes
* Correlation between numerical features and insurance charges

## 🧹 Data Cleaning & Preprocessing

The preprocessing stage includes:

* Checking dataset dimensions and data types
* Checking for missing values
* Removing duplicate records
* Encoding categorical variables
* Converting `sex` into `is_female`
* Converting `smoker` into `is_smoker`
* One-hot encoding regional features

## ⚙️ Feature Engineering

BMI was transformed into categorical groups:

* Underweight
* Normal
* Overweight
* Obese

The categorical BMI features were then encoded for further analysis.

Standardization was also applied to selected numerical features:

* Age
* BMI
* Number of children

## 📈 Statistical Analysis

### Pearson Correlation

Pearson correlation was used to examine the linear relationship between selected features and medical insurance charges.

A higher absolute correlation indicates a stronger linear association. Correlation is used here to identify relationships and does not imply causation.

### Chi-Square Test

Chi-square testing was used to examine associations between categorical features and categorized insurance charges.

A significance level of:

`α = 0.05`

was used for interpreting the statistical results.

## 🔍 Key Observations

The exploratory analysis indicates that:

* Smoking status has a noticeable relationship with medical insurance charges.
* Insurance charges generally increase with age, although the relationship is not purely linear.
* BMI shows a positive association with insurance charges, but the relationship varies across observations.
* Higher-cost observations are particularly concentrated among smokers.
* Male and female insurance-charge distributions show considerable overlap.
* Regional and demographic variables show comparatively weaker or more variable relationships than major factors such as smoking status and age.

## 📁 Project Structure

```
medical-insurance-eda/
│
├── data/
│   └── insurance.csv.zip
│
├── Medical_Insurance_EDA.ipynb
│
├── .gitignore
│
└── README.md
```

## ▶️ How to Run

### 1. Clone the repository

```bash
git clone https://github.com/YOUR-USERNAME/medical-insurance-eda.git
cd medical-insurance-eda
```

### 2. Install dependencies

```bash
pip install numpy pandas matplotlib seaborn scipy scikit-learn jupyter
```

### 3. Launch Jupyter Notebook

```bash
jupyter notebook
```

Open:

```text
Medical_Insurance_EDA.ipynb
```

### 4. Run the notebook

Make sure the dataset is available inside:

```text
data/insurance.csv.zip
```

## 🚀 Future Scope

The processed dataset can be used as a foundation for predictive machine learning tasks, such as building a model to estimate medical insurance charges.

Further work could include:

* Regression model development
* Model comparison
* Feature importance analysis
* Hyperparameter tuning
* Model evaluation using appropriate regression metrics

## 👤 Author

**Tanu Singh**

B.Tech Computer Science & Engineering
