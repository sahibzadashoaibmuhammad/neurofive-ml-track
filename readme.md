# 🚢 Titanic Dataset — Exploratory Data Analysis (EDA)

> **Neurofive Solutions | Machine Learning Track | Internship Task 1**

![Python](https://img.shields.io/badge/Python-3.x-blue?logo=python)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-150458?logo=pandas)
![NumPy](https://img.shields.io/badge/NumPy-Data%20Processing-013243?logo=numpy)
![Google Colab](https://img.shields.io/badge/Google%20Colab-Notebook-orange?logo=googlecolab)
![Status](https://img.shields.io/badge/Status-Completed-success)

---

## 📌 Project Overview

This project is my **first Exploratory Data Analysis (EDA)** task completed as part of the **Neurofive Solutions Machine Learning Track Internship**.

The project explores the well-known **Titanic passenger dataset** to understand its structure, data types, statistical characteristics, and missing values before moving toward data preprocessing and machine learning.

The analysis demonstrates the importance of understanding data before building a machine learning model.

---

## 🎯 Objective

The main objectives of this notebook are to:

- Understand the structure of the Titanic dataset
- Load and inspect the dataset using Pandas
- Explore the first few records
- Examine dataset information and data types
- Generate statistical summaries
- Identify missing values
- Separate numerical and categorical features
- Develop an initial understanding of the dataset
- Prepare a foundation for future machine learning tasks

---

## 📊 Dataset Overview

The dataset contains:

| Property | Details |
|---|---:|
| Rows | **891** |
| Columns | **12** |
| Numerical Features | **7** |
| Categorical Features | **5** |
| Target Variable | **Survived** |

### Dataset Features

- `PassengerId` — Unique passenger identifier
- `Survived` — Survival status
- `Pclass` — Passenger class
- `Name` — Passenger name
- `Sex` — Passenger gender
- `Age` — Passenger age
- `SibSp` — Number of siblings/spouses aboard
- `Parch` — Number of parents/children aboard
- `Ticket` — Ticket information
- `Fare` — Ticket fare
- `Cabin` — Cabin information
- `Embarked` — Port of embarkation

---

## 🔍 Exploratory Data Analysis

The notebook performs several fundamental EDA operations.

### 1. Import Libraries

The project uses:

```python
import pandas as pd
import numpy as np
