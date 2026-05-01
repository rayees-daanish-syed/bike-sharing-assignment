# 🚲 BoomBikes Demand Prediction: Multiple Linear Regression

![Python](https://img.shields.io/badge/Python-3.x-blue.svg)
![Machine Learning](https://img.shields.io/badge/Machine_Learning-Linear_Regression-green.svg)

## 📌 Project Overview
A US bike-sharing provider, BoomBikes, has recently suffered considerable dips in their revenues due to the ongoing Corona pandemic[cite: 4]. The company is finding it very difficult to sustain operations in the current market scenario and aspires to understand the demand for shared bikes among the people after the quarantine situation ends[cite: 4]. This project aims to model the demand for shared bikes with the available independent variables, allowing management to understand how demands vary with different features and adjust their business strategy accordingly to accelerate revenue[cite: 4].

## 🎯 Problem Statement
The primary goal is to understand the factors affecting the demand for these shared bikes in the American market[cite: 4]. Specifically, this project aims to identify:
* Which variables are significant in predicting the demand for shared bikes?[cite: 4]
* How well do those variables describe the bike demands?[cite: 4]

## 🛠️ Workflow & Methodology
The analysis and model building process follows a structured pipeline[cite: 4]:
1. Reading, Understanding, and Quality Check of the data[cite: 4].
2. Visualising the Data[cite: 4].
3. Data Preparation (including dummy variable creation using `drop_first=True` to prevent multicollinearity)[cite: 3, 4].
4. Splitting Data into Train-Test and Scaling[cite: 4].
5. Building a Linear Model (utilizing both Backward Selection and Recursive Feature Elimination)[cite: 4].
6. Residual Analysis to validate model assumptions[cite: 4].
7. Making Predictions[cite: 4].
8. Model Evaluation[cite: 4].

## 📊 Key Findings & Insights
Based on the final Linear Regression model, the top three features contributing significantly towards explaining the demand of the shared bikes are[cite: 3]:
* **`temp`**: This feature has the highest correlation with the target variable, indicating temperature heavily drives bike demand[cite: 3].
* **`Light_snowrain`**: This specific weather situation significantly impacts the volume of bookings[cite: 3].
* **`year`**: This shows a strong positive trend, with 2019 attracting a greater number of bookings than 2018, demonstrating good business progress prior to the pandemic[cite: 3].

Additionally, exploratory data analysis revealed:
* Most bookings were made during the months of May, June, July, August, September, and October[cite: 3].
* The Fall season attracted more bookings overall[cite: 3].
* Clear weather naturally attracted more bookings[cite: 3].

## 🔬 Model Validation
The linear regression model's reliability was validated by checking the following key assumptions during Residual Analysis[cite: 3]:
* **Normality of Error Terms:** Ensured that the error terms (residuals) follow a normal distribution clustered around zero[cite: 3].
* **Multicollinearity:** Verified that predictor variables are not highly correlated to prevent variance inflation[cite: 3].
* **Linearity:** Confirmed a linear relationship between the independent variables and the dependent variable[cite: 3].
* **Homoscedasticity:** Checked that the variance of the residuals remains constant across all levels of the predictor variables without visible patterns[cite: 3].
* **Independence of Variables:** Ensured that the predictor variables used in the regression model are not correlated with each other[cite: 3].

## 📂 Repository Structure
```text
├── bike-sharing-assignment.ipynb         # Main Jupyter Notebook containing the code and linear regression models
├── Bike Sharing Subjective Questions.pdf # Detailed answers to subjective questions regarding the analysis
├── day.csv                               # The dataset containing daily bike demands and weather data
└── README.md                             # Project documentation
