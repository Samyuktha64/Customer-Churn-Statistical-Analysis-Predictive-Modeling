# Customer-Churn-Statistical-Analysis-Predictive-Modeling
Customer churn refers to customers discontinuing their subscription or service. Predicting and understanding churn can help organizations identify customer groups with higher attrition risk and support customer retention strategies.

This project analyzes the Orange Telecom Customer Churn dataset, which contains customer activity and service-related characteristics along with a churn indicator showing whether a customer discontinued the service. The dataset is divided into churn-80 and churn-20 subsets, with the larger dataset intended for model development and the smaller dataset for final model evaluation.

The analysis was performed using IBM SPSS Statistics and combines statistical hypothesis testing, survival analysis, and binary logistic regression to examine factors associated with customer churn and evaluate the discriminatory performance of the predictive model.

**2. OBJECTIVES**

1.To examine the association between customer contract type and churn.

2.To compare monthly charges between churned and retained customers.

3.To analyze customer retention duration across different contract types using survival analysis.

4.To identify important factors associated with the likelihood of customer churn using binary logistic regression.

5.To evaluate the discriminatory performance of the logistic regression model using ROC curve and AUC analysis.

6.To investigate the relationship between contract commitment and technical support adoption.

7.To identify customer characteristics and service patterns associated with higher churn risk.

**3. DATASET: Telecom Customer Churn Dataset**

The dataset contains customer-level information related to customer activity, services, billing, contract characteristics, and churn status.

The available dataset consists of two subsets:

1.churn-80: Used for model development and cross-validation.

2.churn-20: Intended for final testing and model performance evaluation.

The analysis in this project was conducted on the available customer churn data containing 7,043 observations.

**STATISTICAL ANALYSIS**

**4.1 Pearson Chi-Square Test of Independence**

Used to examine whether contract type is associated with customer churn.

Variables: Contract Type and Churn

Test: Pearson Chi-Square

Effect size: Cramér's V

**4.2 Independent Samples t-Test**

Used to compare monthly charges between churned and retained customers.

Because Levene's test indicated unequal variances, Welch's correction was used for the comparison.

**4.3 Kaplan-Meier Survival Analysis**

Used to compare the time-to-churn/retention distribution across different contract types.

A Log-Rank test was used to determine whether the survival distributions differed significantly.

**4.4 Binary Logistic Regression**

Used to model the likelihood of customer churn based on:

Customer tenure

Monthly charges

Contract type

Senior citizen status

Paperless billing

Model performance was assessed using:

Likelihood-ratio Chi-Square
Nagelkerke R²

Classification accuracy

Odds ratios, Exp(B)

ROC curve and AUC

**4.5 Contract and Technical Support Adoption Analysis**

A categorical association analysis was performed to examine the relationship between contract commitment level and technical support adoption, with Bonferroni-adjusted pairwise comparisons.

**RESULTS**
1. Chi-Square: Contract type was significantly associated with churn (χ² = 1184.60, p < .001; Cramér’s V = 0.410).
   
2.t-Test: Churned customers had significantly higher monthly charges ($74.44) than retained customers ($61.27) (p < .001).

3.Kaplan-Meier: Retention differed significantly by contract type (p < .001), with median survival of 12, 44, and 64 months for month-to-month, one-year, and two-year contracts.

4.Logistic Regression: The model was significant (p < .001), explained 37.3% of variance, and correctly classified 79.0% of cases.

5.ROC Analysis: The logistic regression model achieved an AUC of 0.840, indicating good discrimination between churned and non-churned customers.

6.Technical Support: Contract type was significantly associated with technical support adoption (χ² = 1543.47, p < .001; Cramér’s V = 0.331).

**INTERPRETATION**
1.Contract type was significantly associated with customer churn.

2.Customers who churned had higher average monthly charges than retained customers.

3.Retention duration differed significantly across contract types, with longer median survival times for longer-term contracts.

4.The logistic regression model was statistically significant and achieved 79.0% classification accuracy.

5.Contract duration and tenure were associated with lower churn odds.

6.Monthly charges and senior citizen status were associated with higher churn odds.

7.The logistic regression model achieved an AUC of 0.840, indicating good discriminatory performance.

8.Technical support adoption differed significantly across contract commitment levels.

**CONCLUSION**
This project demonstrates the application of statistical methods and predictive modeling to customer churn analysis. The results show that contract type, customer tenure, monthly charges, and customer characteristics are associated with churn behavior.

The survival analysis demonstrated substantial differences in retention duration across contract types, while logistic regression identified significant predictors of churn. The ROC analysis further showed that the predictive model achieved an AUC of 0.840, indicating good discriminatory ability.

Overall, the analysis demonstrates how statistical hypothesis testing, survival analysis, and predictive modeling can be combined to understand customer churn and identify factors associated with customer retention.
