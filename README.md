# Customer Data Exploratory Analysis

## Project Overview

This project presents an **Exploratory Data Analysis (EDA)** of a customer dataset containing demographic, professional, geographic, and salary information.

The objective is to explore the dataset, identify patterns and trends, and investigate relationships between variables such as **age, salary, profession, and city**.

## Objectives

The analysis aims to answer the following questions:

* What is the age distribution of customers?
* What is the salary distribution?
* Are there any missing values or duplicate records?
* Which occupations are most represented?
* Which cities are most represented?
* Is there a relationship between age and salary?
* How does average salary differ across occupations?
* How does average salary differ across cities?
* Which occupations have the oldest customers on average?

## Dataset

The dataset contains **150 customers** and **5 variables**:

| Variable     | Description           | Type        |
| ------------ | --------------------- | ----------- |
| `Nom`        | Customer name         | Categorical |
| `Âge`        | Customer age          | Numerical   |
| `Ville`      | Customer's city       | Categorical |
| `Profession` | Customer's occupation | Categorical |
| `Salaire`    | Customer's salary     | Numerical   |

### Data Quality

* **150 rows**
* **5 columns**
* No missing values
* No duplicate records
* 2 numerical variables
* 3 categorical variables

## Analysis Performed

### 1. Data Exploration

The dataset was initially explored using:

* `head()`
* `shape`
* `dtypes`
* `info()`
* Missing-value analysis
* Duplicate detection

### 2. Descriptive Analysis

Descriptive statistics were calculated for the numerical variables, including:

* Mean
* Standard deviation
* Minimum
* Maximum
* Quartiles

The average customer age is approximately **41.3 years**, while the average salary is approximately **37,154**.

### 3. Distribution Analysis

Histograms were used to visualize:

* Age distribution
* Salary distribution

Box plots were also used to identify potential outliers.

### 4. Outlier Detection

The **Interquartile Range (IQR)** method was used to detect potential outliers.

Three salary observations were identified as potential outliers, including customers with salaries of **0** and **3,053**.

These observations correspond to customers whose occupation is listed as **Chômeur**.

### 5. Categorical Analysis

The number of unique occupations and the distribution of customers across occupations and cities were analyzed.

There are **20 different occupations** in the dataset.

The most represented occupation is **Artisan**, with 14 customers.

The most represented cities are:

* Marseille — 9 customers
* Tours — 9 customers
* Paris — 9 customers

### 6. Correlation Analysis

The Pearson correlation between age and salary is:

**-0.0176**

This indicates that there is **no meaningful linear relationship between age and salary** in this dataset.

### 7. Salary by Occupation

Average salary was calculated for each occupation.

The occupation with the highest average salary is:

**Médecin — approximately 61,421**

Other occupations with relatively high average salaries include:

* Avocat
* Cadre
* Consultant
* Ingénieur

### 8. Salary by City

Average salary was also compared across cities.

The city with the highest average salary in this dataset is:

**Grenoble — approximately 50,372**

### 9. Age by Occupation

Average age was calculated for each occupation.

The occupation with the highest average age is:

**Agriculteur — approximately 49.6 years**

## Key Findings

The analysis produced several main findings:

* The dataset contains **150 customers** with no missing values or duplicate records.
* There are **20 different occupations**.
* **Artisan** is the most represented occupation.
* **Marseille, Tours, and Paris** are the most represented cities.
* **Médecin** has the highest average salary among the occupations.
* **Grenoble** has the highest average salary among the cities.
* **Agriculteur** has the highest average age on average.
* There is **almost no linear correlation between age and salary** (`r = -0.0176`).
* Salary varies considerably across both occupations and cities.

## Technologies and Libraries

The analysis was conducted using Python and the following libraries:

* **Python**
* **Pandas** — data manipulation and analysis
* **NumPy** — numerical operations
* **Matplotlib** — data visualization
* **Seaborn** — statistical visualization

## Project Structure

```text
customer-data-analysis/
│
├── donnees_clients.csv
├── customer_analysis.ipynb
└── README.md
```

## Conclusion

This exploratory analysis provides an initial understanding of the demographic, geographic, professional, and salary characteristics of the customers.

The analysis shows substantial differences in salary across occupations and cities, while **age does not appear to be a useful linear predictor of salary** in this dataset.

This project demonstrates the use of Python for **data cleaning, exploratory analysis, statistical analysis, outlier detection, and data visualization**.
