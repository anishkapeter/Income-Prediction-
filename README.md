## Income Prediction Using Statistical & Machine Learning Models

### Objective
Predict whether an individual earns more than $50K annually using demographic and employment data, and compare classical statistical models with machine learning approaches.

### Business Context
Understanding the drivers of income can help:
- Inform workforce and labor market analysis
- Support policy evaluation and economic research
- Improve fairness and transparency in predictive models

This project analyzes census-style income data to identify key predictors and evaluate multiple modeling strategies.

### Data
- Adult Income dataset (UCI Census-style data)
- Binary response: income (>50K vs ≤50K)
- Mix of numerical and high-cardinality categorical predictors

### Methods
**Exploratory Data Analysis**
- Distributional analysis by income group
- Correlation analysis for numerical predictors
- Interaction exploration across demographic variables

**Feature Selection**
- LASSO regularization for numerical and categorical predictors
- Dummy encoding for high-cardinality categorical variables
- Domain-informed variable inclusion

**Models Implemented**
- Logistic Regression (baseline & interaction-heavy models)
- Quadratic Discriminant Analysis (QDA)
- Random Forest with PCA-reduced continuous features

**Model Evaluation**
- Confusion matrix
- Sensitivity & specificity
- Precision / NPV
- ROC curves and AUROC

### Results Summary
- Logistic regression provided strong interpretability and competitive performance
- QDA achieved balanced sensitivity and specificity with a reduced feature set
- Random forest captured nonlinear patterns but showed lower generalization performance
- Trade-offs between interpretability and flexibility were explicitly evaluated

### Tools & Technologies
- R
- ggplot2, glmnet, caret, pROC
- Logistic regression, LASSO, QDA, Random Forest
- PCA for dimensionality reduction

### Files
- `income_analysis.Rmd`: Full analysis and modeling workflow
- `income_analysis.html`: Rendered report with plots and interpretation

### Key Takeaways
- Feature selection is critical when working with high-cardinality categorical data
- Classical statistical models remain highly competitive for structured tabular data
- Model choice should balance interpretability, performance, and fairness considerations

---
*Completed as part of a graduate-level applied statistics course.*
