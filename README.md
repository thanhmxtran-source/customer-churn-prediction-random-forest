# Customer Churn Prediction with Random Forest

## Overview
This project analyzes customer churn behavior for an e-commerce company using machine learning models to identify customers who are likely to stop using the platform and the factors that contribute to churn. The analysis leverages customer demographics, purchasing behavior, engagement metrics, and satisfaction indicators to support data-driven retention strategies.

This project was completed as part of a group effort with three members. The analysis involved building and evaluating multiple machine learning models to predict customer churn in an e-commerce dataset. Models included K-Nearest Neighbors, Random Forest, and a Gradient Boosting-based classification model developed in SAP Analytics Cloud.

Each team member contributed to different parts of the modeling process. This repository focuses on the Random Forest model, which was one of the primary models used for comparison.

## Objectives
- Clean and preprocess customer churn data for machine learning analysis  
- Transform categorical variables into dummy variables for modeling  
- Explore relationships between customer characteristics and churn behavior  
- Build and evaluate a Random Forest classification model  
- Identify key drivers of customer churn  
- Provide actionable business recommendations to improve customer retention

## Dataset
- **Source:** Kaggle E-commerce Customer Churn Dataset  
- **Size:** 5,630 customer records (4,025 records after data cleaning)
- **Target Variable:** Churn: Indicates whether a customer stayed (0) or churned (1)
- **Key Features:** Demographic, behavioral, and transaction-related features

## Tools
- **Language:** R  
- **Libraries:** ranger, caret, dplyr  
- **Environment:** RStudio
 
## Methodology

### Data Cleaning
- Removed observations containing missing values  
- Reduced dataset size from 5,630 to 4,025 records  

### Feature Engineering
- Converted categorical variables into dummy variables  
- Grouped payment methods into broader categories  
- Removed one dummy variable from each category to avoid multicollinearity  

### Exploratory Data Analysis
- Examined correlations between predictors and churn  
- Analyzed customer behavior patterns through visualizations  
- Identified potential churn indicators before model training
  
### Model Development
- Split data into training (80%), validation (10%), and test (10%) sets  
- Built a Random Forest classifier using the Ranger package  
- Trained multiple decision trees using bootstrap sampling  
- Evaluated model performance using accuracy, sensitivity, specificity, and precision  

## Results
Validation Set:
- Accuracy: 98.51%
- Sensitivity: 93.55%
- Specificity: 99.41%
- Precision: 96.67%

Test Set:
- Accuracy: 97.52%
- Sensitivity: 94.87%
- Specificity: 98.15%
- Precision: 92.50%

## Key Findings
- The Random Forest model demonstrated strong predictive performance and generalized well to unseen data.  
- Customer tenure was one of the strongest indicators of churn, with newer customers more likely to leave.  
- Customers who submitted complaints showed a higher likelihood of churning.  
- Longer periods since the last order were associated with increased churn risk.  
- Product category preferences and customer demographics also contributed to churn behavior.  

## Model Comparison
A comparison of multiple machine learning models was conducted across the team to evaluate performance and identify the most effective approach for churn prediction.

## Business Recommendations
- Develop onboarding and loyalty programs for new customers  
- Address customer complaints quickly through proactive support initiatives  
- Re-engage inactive customers with targeted promotions and personalized offers  
- Monitor high-risk customer segments and implement retention campaigns before churn occurs  

## Project Outcome
The Random Forest model achieved strong predictive performance and was evaluated alongside other models developed within the team. The results demonstrate how machine learning can help e-commerce companies identify at-risk customers and improve retention strategies.
