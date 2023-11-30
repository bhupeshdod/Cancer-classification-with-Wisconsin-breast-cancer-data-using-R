# Cancer-classification-with-Wisconsin-breast-cancer-data-using-R

**Overview** <br>
This repository contains a logistic regression analysis of the Wisconsin breast cancer dataset. The primary objective is to predict breast cancer diagnosis (Benign or Malignant) based on various cellular features obtained from fine needle aspirates of breast masses.

**Data** <br>
The dataset comprises 569 instances with 30 feature columns describing cellular properties, and a binary outcome variable for diagnosis (Benign or Malignant). The features include characteristics like radius, texture, smoothness, and symmetry of cell nuclei, recorded as mean, standard error, and worst values.

**Methodology** <br>
Preprocessing: The data was first processed to address multicollinearity among the features. <br>
Model Building: Utilizing backward step elimination, a logistic regression model was developed. Initial models for mean, standard error, and worst feature values were created and refined, leading to a final model with eight key predictive features.<br>
Assumption Checks: Various tests, including the Variance Inflation Factor (VIF), Logit Linearity test, and Durbin-Watson test, were conducted to validate the model assumptions.

**Key Findings** <br>
The final logistic regression model includes eight significant features.<br>
Multicollinearity and independence of errors were adequately addressed.<br>
Model diagnostics indicated a good fit to the data, with no evidence of lack of fit from the Hosmer-Lemeshow test.


| Variable               | Odds Ratio (OR)   | 2.5 %      | 97.5 %    | Estimate | Std. Error | z value | Pr(>|z|) |
|------------------------|-------------------|------------|-----------|----------|------------|---------|----------|
| (Intercept)            | 8.279e-14         | -41.9632   | -20.8591  | -30.122  | 5.3033     | -5.67995| <0.001   |
| radius_worst           | 2.928             | 0.6947     | 1.54711   | 1.07436  | 0.2142     | 5.01550 | <0.001   |
| smoothness_mean        | 1.286e-57         | -233.258   | -42.3103  | -130.996 | 48.1771    | -2.71905| 0.00655  |
| concavity_mean         | 2.638e+09         | 1.4482     | 42.41813  | 21.693   | 10.3747    | 2.09098 | 0.03653  |
| radius_se              | 1.055e+04         | 4.2742     | 14.94634  | 9.26392  | 2.6026     | 3.55943 | 0.00037  |
| texture_se             | 7.554             | 0.626      | 3.56496   | 2.02201  | 0.7403     | 2.73142 | 0.00631  |
| fractal_dimension_se   | 1.371e-206        | -872.745   | -158.816  | -474.017 | 185.4036   | -2.55668| 0.01057  |
| smoothness_worst       | 7.886e+46         | 54.6958    | 167.763   | 107.984  | 28.61091   | 3.77423 | 0.00016  |
| concave.points_worst   | 9.144e+16         | 11.0346    | 70.1363   | 39.0544  | 14.95191   | 2.61200 | 0.00900  |


**Conclusion** <br>
The analysis successfully identifies significant predictors for breast cancer diagnosis. However, it is emphasized that these findings are based on a specific sample and further research is required for generalization.

Repository Contents
Data Analysis Scripts
Model Development Notebooks
Visualizations and Model Diagnostics
Appendices with detailed statistical test results
