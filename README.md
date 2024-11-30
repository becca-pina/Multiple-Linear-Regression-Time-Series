# Multiple Linear Regression Analysis: Diagnosing Model Assumptions and Predictive Insights

## Table of Contents
1. [Introduction](#introduction)
2. [Dataset Description](#dataset-description)
3. [Objective](#objective)
4. [Methodology](#methodology)
5. [Results](#results)
6. [Dependencies](#dependencies)
7. [Instructions to Run the Code](#instructions-to-run-the-code)
8. [Conclusion](#conclusion)
9. [Contact Information](#contact-information)

---

## Introduction
This project explores and implements a multiple linear regression model to analyze the relationship between a dependent variable \(y\) and a set of independent variables (\(x1, x2, x3\)). The study focuses on evaluating the assumptions of linear regression, diagnosing the model's validity, and making predictions based on test data.

---

## Dataset Description
- **Source**: The dataset is synthetically generated for academic purposes.
- **Size**: 1000 rows and 4 variables.
- **Features**:
  - `y`: Target variable (dependent variable).
  - `x1`, `x2`: Continuous predictor variables.
  - `x3`: Categorical predictor variable with three levels (`A`, `B`, `C`).

The categorical variable (`x3`) was one-hot encoded into `x3_B` and `x3_C` to facilitate regression modeling.

---

## Objective
The primary objectives of this project are:
1. To build a reliable multiple linear regression model.
2. To ensure the model satisfies the Gauss-Markov assumptions:
   - Linearity
   - Homoscedasticity
   - Independence of errors
   - No multicollinearity
   - Normality of residuals
3. To evaluate the model’s predictive accuracy using performance metrics such as:
   - Mean Absolute Error (MAE)
   - Relative Error

---

## Methodology
1. **Exploratory Data Analysis (EDA)**:
   - Investigated the dataset for missing values, outliers, and data types.
   - Visualized relationships using a correlation heatmap and pair plots.
   - Applied one-hot encoding for categorical variables.

2. **Data Cleaning**:
   - Outliers were identified using Z-score and IQR methods.
   - Outliers were retained or removed based on their impact on model performance.

3. **Model Building**:
   - Created an Ordinary Least Squares (OLS) regression model using the training data.
   - Split the dataset into 80% training and 20% test partitions.

4. **Diagnostics**:
   - Performed a range of diagnostics to validate the Gauss-Markov assumptions:
     - **Residual vs. Fitted Values Plot**: To verify linearity.
     - **Scale-Location Plot**: To assess homoscedasticity.
     - **Q-Q Plot**: To check residual normality.
     - **Cook’s Distance**: To identify influential observations.
     - **Breusch-Pagan Test**: To confirm homoscedasticity statistically.
     - **VIF Analysis and Condition Number**: To check multicollinearity.

5. **Evaluation**:
   - Evaluated predictive performance on the test set using MAE and relative error metrics.

---

## Results
- **R-squared**: The model explains 65% of the variance in the target variable.
- **Assumptions**:
  - Linearity, homoscedasticity, independence, and multicollinearity requirements were satisfied.
  - Minor deviations from normality in the residuals were detected but deemed acceptable due to the large sample size.
- **Performance Metrics**:
  - **Mean Absolute Error (MAE)**: 911.53.
  - **Relative MAE (Mean)**: 5.92%.
  - **Relative MAE (Range)**: 7.63%.

Visualizations and diagnostics confirmed the model's validity and stability.

---

## Dependencies
This project requires the following Python libraries:
- `pandas`
- `numpy`
- `matplotlib`
- `seaborn`
- `plotly`
- `statsmodels`
- `scikit-learn`
- `scipy`

Ensure these libraries are installed using `pip install` or a similar package manager.

---

## Instructions to Run the Code
1. Clone the repository:
   ```bash
   git clone <repository-link>
   cd <project-directory>
2. Install dependencies
   ```bash
   pip install -r requirements.txt
3. Run the Jupyter Notebook or Python script:
	- Jupyter Notebook: Open `analysis.ipynb` and execute cells sequentially.
	- Python Script: Run the main script using:
	```bash
	python main.py
4.Outputs include:
	- Diagnostic plots (saved in the /plots directory).
	- Model summary and performance metrics (printed in the terminal).

---

## Conclusion
This project successfully implemented a multiple linear regression model and validated its assumptions. The model demonstrated good predictive accuracy and adhered to the Gauss-Markov conditions. While slight deviations from residual normality were observed, they were not deemed significant enough to compromise model validity.

The analysis provides a solid framework for applying multiple linear regression in real-world scenarios.

---

## Contact Information
For questions or further discussion about this project, feel free to contact:

Name: Rebecca P
Email: [x23436786@student.ncirl.ie]
LinkedIn: [https://www.linkedin.com/in/rebecca-pina/]