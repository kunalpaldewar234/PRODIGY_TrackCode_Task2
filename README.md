# Task 2 — Data Cleaning and Exploratory Data Analysis (EDA) on Titanic Dataset

## Overview
This project performs data cleaning and exploratory data analysis on the Titanic dataset to explore relationships between variables and identify patterns and trends that influenced passenger survival.

## Dataset
- **Source:** Titanic Dataset (titanic-selected-columns.csv)
- **Records:** 891 passengers
- **Key columns:** survived, sex, age, class, fare, embark_town, who

## Steps Performed

### 1. Data Exploration
- Viewed dataset structure using `head()`, `shape`, `info()`, and `describe()`

### 2. Data Cleaning
- Handled missing values — median fill for `age`, dropped rows with missing `embark_town`
- Removed duplicate records
- Detected outliers using IQR method and boxplots
- Capped `fare` outliers using `clip()` to retain data

### 3. Univariate Analysis
- Age distribution (histogram + boxplot)
- Gender distribution
- Passenger class distribution
- Embarkation town distribution

### 4. Bivariate Analysis
- Sex vs Survival
- Age Group vs Survival
- Passenger Category vs Survival
- Class vs Survival

### 5. Multivariate Analysis
- Correlation heatmap using seaborn

## Key Findings
- Female passengers had a significantly higher survival rate than males
- Children (0–12) had the highest survival rate among all age groups
- First-class passengers survived more than second and third-class passengers
- Fare and passenger class show the strongest correlation with survival

## Tools & Libraries
| Library | Purpose |
|---|---|
| Python | Core programming language |
| Pandas | Data manipulation and cleaning |
| NumPy | Numerical operations |
| Matplotlib | Data visualization |
| Seaborn | Statistical data visualization |
