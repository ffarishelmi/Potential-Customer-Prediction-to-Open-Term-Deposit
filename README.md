# Potential Customer Prediction to Open Term Deposit

**Description**

This project analyzes marketing data to identify patterns and builds a machine learning model to predict customer responses to term deposit offers. It includes exploratory data analysis, feature engineering, and model evaluation, providing actionable insights to improve marketing strategies and conversion rates for banks.

# Machine Learning Business Formulation
![image](https://github.com/ffarishelmi/Potential-Customer-Prediction-to-Open-Term-Deposit/blob/main/img/ML%20business%20formulation.png)

# Flowchart
![image](https://github.com/ffarishelmi/Potential-Customer-Prediction-to-Open-Term-Deposit/blob/main/img/Flowchart%20final%20project.png)

# Potential Customer Prediction to Open Term Deposit

## Project Overview

This project begins by analyzing the contributing factors to a successful marketing campaign, focusing on three key areas: identifying customer segments or characteristics of individuals most likely to accept the term deposit offer, determining campaign strategies that yield high conversion rates, and identifying the right timing based on socio-economic conditions for the bank to execute campaigns. Following this analysis, the project builds a machine learning model to predict which potential customers are likely to open a term deposit account. These insights help banks target marketing campaigns more effectively, increasing conversion rates and optimizing marketing budgets by focusing on promising leads.

## Objectives

- Analyze past marketing campaign data to find patterns that result in conversion rates.
- Build a machine learning model to predict the likelihood of a customer opening a term deposit.
- Provide actionable insights to improve marketing strategies and customer targeting.

## Dataset

The dataset used in this project is publicly available for research purposes. It is detailed in the publication by S. Moro, P. Cortez, and P. Rita titled "A Data-Driven Approach to Predict the Success of Bank Telemarketing" published in Decision Support Systems, Elsevier, 62:22-31, June 2014. [Link to dataset](http://archive.ics.uci.edu/ml/datasets/Bank+Marketing).

The data was created by Sérgio Moro (ISCTE-IUL), Paulo Cortez (Univ. Minho), and Paulo Rita (ISCTE-IUL), collected from May 2008 to November 2010, and enriched in 2014 with socio-economic indicators from Banco de Portugal. The dataset includes information about potential customers data, marketing approaches, and socio-economic indicators.

## Methodology

1. **Data Preprocessing**: Cleaned and prepared the data by handling missing values, encoding categorical features, and normalizing numerical data.
2. **Exploratory Data Analysis (EDA)**: Analyzed key features and relationships between them to determine which factors influence a customer's decision to open a term deposit.
3. **Model Building**: Experimented with several machine learning algorithms for classification problems to predict insurance claims.
4. **Model Evaluation**: Evaluated models using recall to choose the best performing model.

## Key Insights

- The barplot analysis shows that while most contacted customers were aged between 28 and 59, Generation Z (aged 17-27) and Boomers (aged 60+) had the highest conversion rates. Therefore, we recommend targeting Generation Z and Boomers.
- Most contacted individuals were married, but single individuals had the highest conversion rates. Singles may have fewer financial constraints compared to married or divorced individuals, making them more likely to invest.
- People with university degrees, professional courses, and basic education (9 years) were contacted most frequently, but those with high school education had a higher conversion rate. This aligns with previous age-related insights, as high school-aged individuals are among those likely to invest.
- Customers with a professional course and a university degree showed significant conversion rates. People with higher education levels may be more inclined to invest due to better financial literacy and higher income levels.
- Most contacted customers worked in administrative, blue-collar, or technical roles, but students and retirees had the highest conversion rates (above 25%). This supports previous findings that Generation Z and Boomers are more likely to accept term deposit offers.
- The analysis shows that customers with a history of loan default did not accept term deposit offers. Despite the limited data, it is advisable not to target individuals with a history of loan default, as they are less likely to accept.
- Contrary to our hypothesis, both individuals with and without personal loans tend to make similar decisions regarding term deposit acceptance.
- A significant relationship exists between housing loans and term deposit decisions. While many with housing loans accepted the offer, there was no clear pattern.
- The analysis shows that customers were more likely to respond positively when contacted via cellular phones compared to traditional phones. This trend aligns with the growing popularity of mobile phones over landlines during the 2008-2010 period.
- The analysis of socio-economic indicators suggests that banks should focus on factors such as employment variation, total employment, inflation, and Euribor rates, while customers are more influenced by consumer confidence indices when deciding to invest.
- Scatterplot analysis shows that longer call durations (at least 7 minutes) generally result in higher conversion rates. Initial longer calls are more effective, while repeated short calls do not improve outcomes and may waste resources.

## Tools Used

- **Basic Libraries**: NumPy, Pandas
- **Visualization**: Matplotlib, Seaborn
- **Data Processing**: Scikit-learn (ColumnTransformer, Pipeline, OneHotEncoder, StandardScaler)
- **Modeling**: Scikit-learn, XGBoost, LightGBM, CatBoost
- **Model Evaluation**: Scikit-learn (confusion\_matrix, classification\_report, roc\_auc\_score)

## How to Run

1. Clone the repository:
   ```sh
   git clone https://github.com/ffarishelmi/Potential-Customer-Prediction-to-Open-Term-Deposit.git
   ```
2. Install the required library:
   ```sh
   pip install scipy
   pip install scikit-learn
   pip install imbalanced-learn
   pip install xgboost
   pip install lightgbm
   pip install catboost
   pip install statsmodels
   pip install shap
   ```
3. Run potential_customer_prediction.ipynb file the notebook environment you are using.

## Conclusion

Data analysis was conducted using various statistical methods, and a model was built using Logistic Regression. The model supports the data analysis findings and can help reduce the bank's losses by a factor of 10 compared to potential profits. The bank stands to gain a profit margin of 24% if the model is used to plan future campaigns. Assumptions such as phone costs, deposit and loan interest rates, and the range of funds customers can allocate for deposits can be adjusted according to current conditions. Patterns and factors influencing customers' decisions to accept term deposit offers have been identified.

## Next Steps

- Model performance can be further improved by increasing the number of parameter combinations trained in RandomizedSearchCV. Due to limited computational resources, only 120 combinations out of 1200 possible parameter combinations were tested.
- Ensure that in the future, the management team instructs staff to store all potential customer data, avoiding any unknown values. As explained in the data analysis phase, features with unknown values have implications on whether a customer is likely to accept the term deposit offer.
- If management wants insight into how monthly effects impact conversion rates, it is advisable to run campaigns evenly throughout the year. Although this requires a significant budget and the return may not be guaranteed, data can be considered an investment for the company.

Feel free to contribute by suggesting improvements or adding new features!
