## About 
This project focuses on Project 2 of Data 201, implementing Linear Regression to explore the relationship between hours worked per week, productivity scores, employment type, and well-being scores.

## Data Source
The dataset is sourced from Kaggle and titled "Remote Work Productivity". The key variables in this dataset are:

-Hours Worked Per Week
-Productivity Score
-Well-Being Score
-Employment Type (Two categories: Remote Work & Onsite Work)

## Dataset Overview:
Total cases: 1001
Each case represents an employee with the following variables:
ID Number
Hours Worked Per Day
Well-Being Score
Work Type (binary: Onsite vs Remote)

## Exploratory Data Analysis (EDA)
The EDA results provide insights into employee work patterns and well-being:

## Key Findings:
Working Hours: Most employees work between 35 to 45 hours per week.
Productivity Distribution:

The distribution of productivity scores follows a normal distribution as shown in the histogram.
Correlation Findings:

A strong correlation is observed between hours worked per week and a binary encoded employment type variable (onsite workers vs remote workers).
Boxplots Analysis:

Hours Worked by Work Type:
Employees in office settings exhibit higher counts of working hours per week compared to their remote counterparts.
Productivity vs. Employment Type:
Median productivity scores are higher among remote workers compared to onsite workers. Specifically:
Median productivity scores for remote workers are above 70.
Median productivity scores for onsite workers are less than 70.

## Linear Regression Model
The linear regression model evaluates how hours worked per week, productivity scores, and employment type impact well-being scores.

Model Results:
R² Score: 0.1088
Indicates that only 10.88% of the variance in well-being scores is explained by the independent variables.
Mean Squared Error (MSE): 170.43
Suggests that the predictions are not highly accurate, and residuals have high variability.
Residual Analysis:
Analysis shows high variability in residuals, indicating that the model does not accurately predict well-being scores.
### Key Findings from Linear Regression Analysis
The model's coefficients highlight important insights into the relationships between variables:

Coefficients:
[-0.09645701, -0.01616481, -10.34311591]
Intercept:
74.24351283427022
Interpretation:
The coefficient value of -10.34 indicates that working in an office is negatively associated with the well-being score compared to working remotely. This suggests that employees working in office settings experience lower well-being scores, assuming all other factors remain constant.
📊 Visualizations
Pair Plot of Variables
A pair plot was used to visualize the relationships between the following variables:

Employment Type (onsite/remote)
Hours Worked Per Week
Productivity Scores
Well-Being Score (target variable)
The pair plot provides insights into patterns and trends across these variables, particularly focusing on how employment type impacts well-being.

## Conclusion
The linear regression model highlights limited explanatory power, suggesting that:

Independent variables do not fully capture the variance in well-being scores.
Further exploration (e.g., non-linear modeling or feature engineering) could provide a more accurate model.
The visualizations and statistical analysis offer a foundational understanding of how hours worked, productivity and employment type interact and impact well-being among employees.

## Acknowledgments
Dataset Source: Kaggle - Remote Work Productivity
Tools Used: matplotlib, seaborn, pandas, scikit-learn, and numpy
