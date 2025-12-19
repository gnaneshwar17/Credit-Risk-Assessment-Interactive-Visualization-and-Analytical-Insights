High Level Data Description : 
This dataset is a synthetic loan portfolio focused on modeling the likelihood of loan default at the individual borrower level.​

Structure and target The file is a flat CSV where each row represents a unique loan, identified by LoanID, with a binary target variable Default (0 = no default, 1 = default). The predictors mix numerical and categorical features describing borrower demographics, credit profile, and loan contract terms.​

Key numerical variables Core continuous fields include borrower Age, Income, LoanAmount, CreditScore, MonthsEmployed, NumCreditLines, InterestRate, LoanTerm, and DTIRatio (debt-to-income ratio). These cover affordability, leverage, credit experience, and price of credit, which are typical drivers in credit risk modeling.​

Key categorical variables Several categorical columns capture socioeconomic and relationship information: Education (e.g., High School, Bachelor's, Master's, PhD), EmploymentType (Full-time, Part-time, Self-employed, Unemployed), and MaritalStatus. Additional binary flags describe household and loan context: HasMortgage, HasDependents, LoanPurpose (Home, Auto, Business, Education, Other), and HasCoSigner.

Quick Summary :
Summarize the project in a quick paragraph
This project builds an end-to-end credit risk assessment framework that combines rich exploratory visualizations with a full machine learning pipeline for default prediction. It starts by loading a retail loan dataset and creating professional, business-oriented figures: categorical default breakdowns, correlation and risk-segmentation views, and an Expected Credit Loss (PD–LGD–EAD) analysis, plus approval-rate and profitability curves across decision thresholds. On the modeling side, it engineers risk-focused features, handles class imbalance (e.g., with SMOTE), and trains a suite of models (from logistic regression to advanced gradient-boosting and ensemble methods), then compares them using consistent metrics and validation. Finally, it links model probabilities to business decisions through threshold optimization and cost–benefit analysis, so that risk, return, and approval policies can be quantitatively aligned.
