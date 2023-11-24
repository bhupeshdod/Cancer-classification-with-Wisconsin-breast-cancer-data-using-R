# Cancer-classification-with-Wisconsin-breast-cancer-data-using-R

Overview
This repository contains a logistic regression analysis of the Wisconsin breast cancer dataset. The primary objective is to predict breast cancer diagnosis (Benign or Malignant) based on various cellular features obtained from fine needle aspirates of breast masses.

Data
The dataset comprises 569 instances with 30 feature columns describing cellular properties, and a binary outcome variable for diagnosis (Benign or Malignant). The features include characteristics like radius, texture, smoothness, and symmetry of cell nuclei, recorded as mean, standard error, and worst values.

Methodology
Preprocessing: The data was first processed to address multicollinearity among the features.
Model Building: Utilizing backward step elimination, a logistic regression model was developed. Initial models for mean, standard error, and worst feature values were created and refined, leading to a final model with eight key predictive features.
Assumption Checks: Various tests, including the Variance Inflation Factor (VIF), Logit Linearity test, and Durbin-Watson test, were conducted to validate the model assumptions.

Key Findings
The final logistic regression model includes eight significant features.
Multicollinearity and independence of errors were adequately addressed.
Model diagnostics indicated a good fit to the data, with no evidence of lack of fit from the Hosmer-Lemeshow test.

Conclusion
The analysis successfully identifies significant predictors for breast cancer diagnosis. However, it is emphasized that these findings are based on a specific sample and further research is required for generalization.

Repository Contents
Data Analysis Scripts
Model Development Notebooks
Visualizations and Model Diagnostics
Appendices with detailed statistical test results
