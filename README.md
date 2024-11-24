# **Bank Customer Churn Analysis**

## **Project Overview**

This project aims to analyze customer churn in a banking environment using data science techniques. By understanding which group of customers are likely to churn, the bank can take preventive actions to improve retention and customer satisfaction. The analysis involves exploring customer behavior, identifying the key factors contributing to churn, and understanding the factors influencing the likelihood of customer attrition.

## **Dataset Description**

The dataset used for this project consists of customer data from a bank. It includes both demographic and transactional details about customers. The dataset contains the following columns:

- `CustomerID`: Unique identifier for each customer.
- `Gender`: The gender of the customer.
- `Age`: Age of the customer.
- `Balance`: The current balance of the customer's account.
- `NumOfProducts`: Number of products the customer is using with the bank.
- `HasCrCard`: Whether the customer has a credit card (1 if yes, 0 if no).
- `IsActiveMember`: Whether the customer is an active member of the bank (1 if yes, 0 if no).
- `EstimatedSalary`: The estimated salary of the customer.
- `Exited`: The target variable indicating whether the customer has churned (1 if yes, 0 if no).

## **Data Cleaning & Preprocessing**

1. **Handling Missing Values**: Missing values were checked for each column, and appropriate methods were used to handle them:
   - For numerical columns, missing values were imputed using the mean.
   - For categorical columns, missing values were imputed with the most frequent category.
   
2. **Feature Encoding**: The categorical variables such as `Gender` and `HasCrCard` were encoded using label encoding.

3. **Feature Scaling**: Features like `Balance`, `EstimatedSalary`, and `Age` were scaled using StandardScaler to bring all numerical features to the same scale for better model performance.

4. **Feature Engineering**: New features such as `TotalProducts` (sum of products used by a customer) were derived to enrich the analysis.

## **Exploratory Data Analysis (EDA)**

The key insights from the exploratory data analysis are as follows:
- The majority of customers who churned are younger and have fewer products with the bank.
- There is a higher churn rate among customers with lower account balances.
- Active members are less likely to churn compared to inactive ones.
- Gender does not have a significant impact on churn, but age and balance are key factors.

**Visualizations**:
- Churn distribution by gender, age, balance, and activity status.
- Correlation heatmap to identify relationships between numerical features.
- Bar plot to compare the churn rate across different customer products.


## **Conclusion**

The analysis provides valuable insights into the factors driving customer churn at the bank. The most influential factors include account balance, number of products, and activity status.

## **Future Work**

1. **Customer Segmentation**: Segmenting customers into different groups based on churn risk to tailor retention strategies.
2. **Additional Features**: Incorporating transaction history or customer service interactions to enhance model performance.
3. **Real-time Prediction**: Deploying the model in a real-time system to predict churn and take action instantly.

## **Technologies Used**

- **Python**: The primary programming language used for the analysis.
- **Pandas**: For data manipulation and cleaning.
- **Matplotlib, Seaborn**: For data visualization.

---
