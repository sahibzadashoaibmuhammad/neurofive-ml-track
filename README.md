# Titanic Survival Prediction Using Logistic Regression

## Overview

This project was completed as part of the **Neurofive Solutions – Machine Learning Internship Track**.

The objective of this task was to build a binary classification model that predicts whether a passenger survived the Titanic disaster. A **Logistic Regression** model was trained using selected passenger features, with categorical variables encoded using **OneHotEncoder**.

The project demonstrates the fundamental Machine Learning workflow, from data preparation and feature engineering to model training and evaluation.

---

## Objectives

The main objectives of this project were to:

- Prepare the Titanic dataset for Machine Learning
- Handle missing values
- Select relevant features and the target variable
- Split the dataset into training and testing sets
- Encode categorical features
- Train a Logistic Regression classification model
- Generate predictions on unseen test data
- Evaluate the model using accuracy
- Analyze the model using a confusion matrix

---

## Dataset

The project uses the **Titanic - Machine Learning from Disaster** dataset.

The original training dataset contains:

- **891 observations**
- **12 features**

The target variable is:

`Survived`

| Value | Meaning |
|---|---|
| 0 | Did not survive |
| 1 | Survived |

---

## Data Preprocessing

Before training the model, the dataset was prepared using the following steps:

### Missing Values

- Missing values in `Age` were replaced with the median age.
- Missing values in `Embarked` were replaced with the most frequent value (mode).
- The `Cabin` column was removed because it contained a large proportion of missing values.

### Feature Selection

The following features were selected for model training:

- `Pclass`
- `Sex`
- `Age`
- `SibSp`
- `Parch`
- `Fare`
- `Embarked`

The following columns were excluded because they were identifiers or not necessary for this model:

- `PassengerId`
- `Name`
- `Ticket`

---

## Train-Test Split

The dataset was divided into training and testing sets using `train_test_split`.

- **80%** of the data was used for training.
- **20%** was used for testing.
- `random_state=42` was used for reproducibility.
- `stratify=y` was used to preserve the target class distribution.

### Dataset Split

- Training samples: **712**
- Testing samples: **179**

---

## Categorical Feature Encoding

Machine Learning algorithms require numerical input. Therefore, categorical features were transformed using **OneHotEncoder**.

The following categorical features were encoded:

- `Sex`
- `Embarked`

`handle_unknown="ignore"` was used to safely handle categories that may not appear in the training data.

---

## Machine Learning Model

### Logistic Regression

**Logistic Regression** was selected as the classification algorithm because the target variable contains two possible outcomes: survived or did not survive.

The model was implemented using a Scikit-learn Pipeline that combines preprocessing and classification.

### Prediction Target

```text
Survived
