# Fraud-Detection-in-Banking-systems
Machine Learning models to create possibility of detecting fraud and analysis.
Credit Card Customer Analysis
	
Credit Card Companies are facing a huge competition in the market space for having people take credit short time. The deals provided in the market space help the customer gain short term benefit for spending a certain amount on the card. This has been a major problem for our company.  So, we’re performing and analysis for credit card to recognize the patterns for credit cards to have long time customer and focus on retaining customer for a long-term benefit. 

Action Plan:
•	Credit Card Company is facing problems on loosing credit card customers.
•	Requirement of an individual to be able to recognize habits leading to loss of customer.
•	Study the statistics of patterns which affect the clients on regular basis. 
•	Proactively take measures to report problems and identify patterns
•	Take action by offering better services to retain the customer. 
The data set we used was from BOA, and we used a bank churners CSV file to utilize the data and collaborate for the action plan. 
Secondly, we looked at the data and found different categories of files to study and differentiate for the customer recollection. 
We found out a need for 20 different categories and based on that we used different models such as SVM, KNN, and logistic regression, 
random forest to find out the best performing model and have a decision-making process based on results.
There are different terms which we used in the coding to find out the customers spending habits and what they spent on for most of their expenses. 
There were 10 patterns where foods and travel were the most incurred expense, we saw in the models we created. 
Through which we utilized random forest to predict the best possibility of features which would help us give an open perspective for making our decision easier.
	The coding part was a difficult process to find out the best performing model we were getting a lot of errors to find out best performing model. 
  After a lot of errors, we came to a conclusion of our best performing model which was random forest as well with an accuracy of 95%. 
  Whereas the accuracy for SVM, KNN, and Logistic regression was 93%, 91%, 90% respectively. 
	For conclusion, we concluded that the female customers were the most reliable one who stayed long-terms and giving them credit
  boosted the highest of the revenue. 
  Furthermore, we also find out the people who were college drop out where most of the people to churn out from the credit card company. Giving them credit would be the number one consequence for not having the profit on the sheets. Lastly, college student were the ones who did not make payments on time and lead to long-term high interests rates which gave more revenue to the company. 


# Bank Customer Churn Analysis Summary

## Project Overview
This project appears to be an analysis of bank customer churn using a dataset called "BankChurners.csv". The analysis includes data preprocessing, exploratory data analysis (EDA), feature engineering, and machine learning model implementation (specifically logistic regression) to predict customer churn.

## Key Components

### 1. Data Preprocessing
- Initial dataset had 10,127 rows and 23 columns
- Removed unnecessary columns including client numbers and Naive Bayes classifier columns
- Checked for and handled missing values (none found)
- Encoded categorical variables using techniques like LabelEncoder and one-hot encoding

### 2. Exploratory Data Analysis (EDA)
- Visualized distribution of various features including:
  - Customer age
  - Gender distribution
  - Income categories
  - Education levels
  - Marital status
  - Credit card categories
- Created correlation heatmaps to understand relationships between variables
- Analyzed the balance between churned and non-churned customers

### 3. Feature Engineering
- Removed highly correlated features to reduce multicollinearity
- Used Variance Inflation Factor (VIF) to identify and remove features with high multicollinearity
- Standardized numerical features using StandardScaler

### 4. Machine Learning Model
- Implemented Logistic Regression for predicting customer churn
- Used SMOTE (Synthetic Minority Over-sampling Technique) to balance the dataset
- Achieved a model accuracy of approximately 90.7%

### 5. Model Interpretation
- Analyzed feature importance using odds ratios from the logistic regression model

## Key Insights

1. **Customer Demographics**: 
   - The age distribution of customers is roughly normal, centered around 46 years old.
   - There's a slight gender imbalance, with more female customers than male.

2. **Income and Education**:
   - The largest income category is "Less than $40K", followed by "60K" and "80K".
   - There's a positive correlation between education level and income.

3. **Churn Factors**:
   - Income category is a strong predictor of churn, with "Unknown" income category having the highest odds ratio.
   - Education level also plays a significant role, with "Uneducated" customers having higher odds of churning.
   - Marital status affects churn, with married customers more likely to churn than single or divorced customers.
   - Gender has an impact, with male customers more likely to churn than female customers.

4. **Card Usage**:
   - The vast majority of customers use Blue cards, with very few Gold or Platinum cardholders.
   - Card category doesn't seem to be a strong predictor of churn.

5. **Customer Engagement**:
   - Total relationship count (number of products with the bank) is positively correlated with retention.
   - Months of inactivity and number of contacts are negatively correlated with retention.

6. **Financial Behavior**:
   - Credit limit and total revolving balance have minimal impact on churn prediction.
   - Transaction count has a slight positive correlation with retention.

## Recommendations

1. **Target High-Risk Segments**: Focus retention efforts on customers with unknown income, lower education levels, and married individuals, as they show higher churn risk.

2. **Improve Customer Engagement**: Develop strategies to increase the total relationship count and reduce inactive months, as these factors are associated with lower churn rates.

3. **Personalized Services**: Create tailored products or services for different income and education segments to improve retention across all customer groups.

4. **Gender-Specific Strategies**: Develop targeted retention strategies for male customers, who show a higher likelihood of churning.

5. **Investigate Income Reporting**: The high churn rate for customers with "Unknown" income suggests a need to improve income data collection or to understand why these customers are not reporting their income.

6. **Transaction Encouragement**: Implement programs to encourage more frequent transactions, as higher transaction counts are associated with lower churn rates.

7. **Further Analysis**: Consider exploring more advanced machine learning models (e.g., Random Forests, Gradient Boosting) to potentially improve prediction accuracy and gain more nuanced insights into churn factors.
