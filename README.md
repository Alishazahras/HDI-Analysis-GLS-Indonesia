# Assessing Human Development in Indonesia Using Generalized Least Squares (GLS) Regression

## Project Overview
This project analyzes the factors influencing Indonesia's Human Development Index (HDI) using a Generalized Least Squares (GLS) Regression model. The primary goal is to understand the impact of the workforce percentage and high school graduation rate on the HDI in various regions across Indonesia. The GLS model is employed to address issues of heteroscedasticity and autocorrelation, improving the reliability and accuracy of the regression analysis compared to conventional methods like Ordinary Least Squares (OLS).

## Objectives
- Examine the relationship between HDI, workforce percentage (WFP), and high school graduation rate (HSC).
- Mitigate potential issues in regression assumptions, such as heteroscedasticity and autocorrelation, using the GLS model.
- Provide insights for policymakers in formulating strategies to improve HDI in Indonesia.

## Data
The dataset for this study was sourced from Badan Pusat Statistik (BPS) and includes:

- Human Development Index (HDI): A composite measure of health, education, and standard of living.
- Workforce Percentage (WFP): The percentage of the population actively participating in the workforce.
- High School Graduation Rate (HSC): The percentage of the population that has completed high school.

## Key Variables :
- Dependent Variable (Y): HDI
- Independent Variables (X1): Workforce Percentage (WFP)
- Independent Variables (X2): High School Graduation Rate (HSC)
The dataset consists of 34 observations, representing the provinces of Indonesia, for the year 2022.

## Methodology
1. **Model Selection**

   We initially apply a Multiple Linear Regression (MLR) model to understand the relationship between the variables. However, due to detected autocorrelation in the residuals, we transition to a Generalized Least Squares (GLS) Regression model.
3. **Regression Assumptions**

   Before implementing the GLS model, the following assumptions are tested:
      - Normality: Checked using the Lilliefors test.
      - Homoscedasticity: Tested using the Breusch-Pagan test.
      - Independence: Checked using the Durbin-Watson test.
      - Multicollinearity: Tested using the Variance Inflation Factor (VIF).
5. **Model Equation**

   The final GLS regression model is as follows:

   $$Y = 53.44 + 0.12$$ x $$WFP + 0.21$$ x $$HSC$$

   Where :
   - $$Y$$ = HDI
   - $$WFP$$ = Workforce Percentage
   - $$HSC$$ = High School Graduation Rate
7. **Software and Tools**

   The project is conducted using RStudio with the following R packages:
   - `nlme`
   - `car`
   - `lmtest`
   - `nortest`

## Results
**Key Findings:**
- Both Workforce Percentage (WFP) and High School Graduation Rate (HSC) are statistically significant predictors of HDI.
- Higher workforce participation and high school graduation rates are associated with increased HDI values in Indonesian provinces.
- The Generalized Least Squares (GLS) model effectively mitigates autocorrelation, providing more reliable results compared to the traditional linear regression model.

**Performance Metrics:**
- Adjusted R-squared of 0.81, indicating the model explains 81% of the variability in HDI.
- Akaike Information Criterion (AIC) and Bayesian Information Criterion (BIC) values suggest that the full model (WFP + HSC) provides the best fit.

## Conclusion
The results of this analysis provide valuable insights into the factors that significantly influence Indonesia’s HDI. The use of GLS regression improves the robustness of the findings, making this analysis a valuable resource for policymakers to focus on improving education and workforce participation to drive human development in Indonesia.

## Contributors
2501971742 - Alisha Zahra Saadiya

2502027301 - Dira Abiyyu Bagaspati

2502042164 - Ilham Hadi Shahputra
