# Access-Inequalities-in-French-Higher-Education



This repository contains two complementary projects—one focusing on econometrics and the other on statistics—analyzing inequalities in access to higher education in France. These projects leverage data from Parcoursup 2022, the French higher education admission platform, to explore key socio-economic and geographical factors influencing admissions.

---

## Projects Overview

### 1. **Econometrics Project**
#### Objective:
To model and analyze the factors influencing admission rates in higher education programs in France, focusing on identifying structural inequalities and understanding the dynamics of access.

#### Data Source:
[Parcoursup 2022 data](https://data.enseignementsup-recherche.gouv.fr/explore/dataset/fr-esr-parcoursup/information/)

#### Key Analyses:
1. **Model Specification**:
   - The dependent variable is the **admission rate** (`percentage_access_rate`).
   - Explanatory variables include:
     - **Scholarship rate (`percentage_admitted_withscholarship`)**: Proportion of admitted students who are scholarship holders.
     - **Regional admissions (`percentage_admitted_sameacademy`)**: Proportion of admitted students from the same academy as the program.
     - **General Baccalaureate rate (`percentage_admitted_generalbac`)**: Proportion of admitted students with a general high school diploma.
     - **Program selectivity (`selectivity_indicator`)**: A binary variable indicating whether a program is selective or not.

2. **Descriptive Statistics**:
   - Exploration of variable distributions, including histograms, boxplots, and correlation analysis.
   - Examination of disparities in admission rates between selective and non-selective programs.

3. **Model Estimation**:
   - A **Multiple Linear Regression Model (OLS)** is used to estimate the impact of explanatory variables on admission rates:
     - \( Y = \beta_0 + \beta_1 X_1 + \beta_2 X_2 + \beta_3 X_3 + \epsilon \)
     - Where \( X_1 \), \( X_2 \), and \( X_3 \) represent the scholarship rate, regional admissions rate, and general baccalaureate rate, respectively.
   - Model refinement through significance testing and elimination of insignificant variables.

4. **Structural Analysis**:
   - **Chow Test**: To evaluate structural breaks in the model between selective and non-selective programs.
   - Separate models are estimated for each program type based on the results.

5. **Error Diagnostics**:
   - **Autocorrelation Detection**:
     - Durbin-Watson test and Breusch-Godfrey test to check for first-order autocorrelation.
   - **Heteroskedasticity Tests**:
     - White test and Goldfeld-Quandt test for heteroskedasticity.
   - Correction of detected issues to ensure robust results.

6. **Final Model**:
   - The final model explains the variability in admission rates using the most significant explanatory variables.
   - Interpretations of coefficients provide insights into the marginal effects of key factors on admission rates.

---

### 2. **Statistics Project**
#### Objective:
To analyze inequalities in access to higher education through descriptive and inferential statistical methods.

#### Key Analyses:
1. **Descriptive Statistics**:
   - Summary statistics and visualizations of admission rates based on socio-economic and geographical factors.
   - Comparisons between selective and non-selective programs.

2. **Confidence Intervals**:
   - Estimation of confidence intervals for admission rates across different categories (e.g., gender, scholarship holders).

3. **Inferential Tests**:
   - Hypothesis tests to evaluate differences in admission rates between key groups (e.g., regional vs. non-regional candidates).

4. **Equity Analysis**:
   - Exploration of fairness in admissions, focusing on socio-economic and regional disparities.

---

## Repository Structure

