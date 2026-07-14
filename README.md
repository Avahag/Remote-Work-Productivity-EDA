# Remote Work Productivity Analysis Using Linear Regression

## About

This project applies **multiple linear regression** to analyze the relationship between several independent variables and a target outcome. The analysis includes data cleaning, exploratory data analysis (EDA), data visualization, model development, and evaluation to identify patterns within the dataset and assess the model's predictive performance.

The project also explores correlations between variables, interprets regression coefficients, and evaluates model accuracy using standard performance metrics such as **R²** and **Mean Squared Error (MSE)**. The findings provide insights into the factors associated with the target variable while highlighting opportunities for future model improvements.

---

## Dataset

**Source:** Kaggle – *Remote Work Productivity*

### Variables
- Hours Worked Per Week
- Productivity Score
- Well-Being Score
- Employment Type (Remote or Onsite)

### Dataset Overview
- **Total observations:** 1,001 employees
- Each record represents one employee and includes:
  - Employee ID
  - Hours Worked Per Week
  - Productivity Score
  - Well-Being Score
  - Employment Type (Remote or Onsite)

---

## Exploratory Data Analysis (EDA)

The exploratory data analysis (EDA) was conducted to understand the relationships between employee work habits, productivity, and well-being.

### Key Findings

### Working Hours
- Most employees work between **35 and 45 hours per week**.

### Productivity Distribution
- Productivity scores follow an approximately **normal distribution**.

### Correlation Analysis
- A noticeable relationship exists between **hours worked per week** and **employment type**.

### Boxplot Analysis

#### Hours Worked by Employment Type
- Onsite employees generally work **more hours per week** than remote employees.

#### Productivity by Employment Type
- Remote employees tend to have **higher productivity scores** than onsite employees.
- Median productivity score:
  - **Remote employees:** Above 70
  - **Onsite employees:** Below 70

---

## Linear Regression Model

A multiple linear regression model was developed to predict **well-being scores** using the following predictors:

- Hours Worked Per Week
- Productivity Score
- Employment Type

### Model Performance

| Metric | Value |
|---------|------:|
| R² Score | 0.1088 |
| Mean Squared Error (MSE) | 170.43 |

### Interpretation

- The model explains approximately **10.9%** of the variation in employee well-being.
- The relatively high MSE indicates that prediction errors remain substantial.
- Overall, the model has **limited predictive power**, suggesting that additional variables may influence well-being.

---

## Regression Coefficients

### Coefficients

```text
Hours Worked Per Week:  -0.09645701
Productivity Score:     -0.01616481
Employment Type:       -10.34311591
```

### Intercept

```text
74.24351283427022
```

### Interpretation

The employment type coefficient (**-10.34**) suggests that, after controlling for the other variables, employees working **onsite** are predicted to have well-being scores approximately **10 points lower** than employees working **remotely**.

---

## Visualizations

The project includes several visualizations to better understand the data, including:

- Histograms
- Boxplots
- Correlation analysis
- Pair plots

### Pair Plot

The pair plot illustrates relationships among:

- Employment Type
- Hours Worked Per Week
- Productivity Score
- Well-Being Score

These visualizations help identify trends, distributions, and potential relationships before modeling.

---

## Conclusion

The linear regression model demonstrates that:

- Hours worked, productivity, and employment type explain only a small portion of employee well-being.
- Additional factors likely influence well-being and should be included in future analyses.
- More advanced modeling techniques, such as polynomial regression, decision trees, or feature engineering, may improve predictive performance.

Overall, this project provides a foundational analysis of how workplace characteristics relate to employee well-being using linear regression.

---

## Technologies Used

- Python
- pandas
- NumPy
- scikit-learn
- Matplotlib
- Seaborn

---

## Acknowledgments

- **Dataset:** Kaggle – *Remote Work Productivity*
- **Course:** DATA 201
