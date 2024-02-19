<b>European Call Option Pricing Prediction<br>
Introduction<br>
This project focuses on predicting European call option values using machine learning models. The prediction models utilize variables from the Black-Scholes (BS) formula, including current option value (Value), current asset value (S), strike price of the option (K), annual interest rate (r), and time to maturity (tau). The project involves building regression models to predict option values and classification models to categorize whether the Black-Scholes equation's prediction overestimates or underestimates the option value.<br>

Executive Summary<br>
The project aims to enhance investment decision-making by detecting whether traditional statistical methods (like the Black-Scholes equation) overestimate or underestimate option prices. The best-performing models identified are the Random Forest regressor (with a mean R-squared of 0.9959) for predicting option values and Boosting classifier (with a mean classification error of 6.57%) for classifying Black-Scholes predictions.<br>

Approach<br>
Data Cleaning & Pre-processing<br>
The initial step involves cleaning the data by removing null values and outliers. Outliers are identified based on implausible values for predictors such as time to maturity and strike price. Additionally, the 'BS' variable indicating option price momentum is converted from "over" and "under" to 1 and 0, respectively, for classification purposes. Data pre-processing includes standardizing and normalizing predictors and creating K-fold Cross-Validation for regression and classification problems.<br>

Regression Model Selection<br>
Various regression models, including KNN regression, Decision Tree regression, Random Forest regression, Boosting regression, and SVM regression, are evaluated based on the mean R-squared of 5-fold Cross-Validation. The Random Forest regression model performs the best, with a mean R-squared of 0.9959, and is chosen for predicting option values.<br>

Classification Model Selection<br>
Different classification models, such as KNN classifier, logistic regression, LDA classifier, Naive Bayes classifier, Decision Tree classifier, Random Forest classifier, Boosting classifier, and SVM classifier, are compared based on the mean classification error of Stratified 5-fold Cross-Validation. The Boosting classifier yields the lowest mean classification error of 6.57% and is selected for classifying Black-Scholes predictions.<br>
Conclusion<br>
Machine learning models offer potential improvements over traditional statistical methods in predicting option values. The identified models demonstrate high accuracy, indicating their potential utility in investment decision-making and risk management scenarios.<br>

Business Understandings<br>
Accurate option pricing is crucial for informed investment decisions. Machine learning models can potentially outperform traditional models like Black-Scholes by capturing complex relationships and adapting to changing market conditions. However, it's essential to consider the limitations of the dataset and model applicability in real-world scenarios.<br>
