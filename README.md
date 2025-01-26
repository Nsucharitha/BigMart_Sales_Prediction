# BigMart_Sales_Prediction


# **BigMart Sales Prediction Project**

## **Overview**
This project aims to predict product sales at BigMart stores using various machine learning models, including a novel **Clustering-Enhanced XGBoost** approach. The primary objective is to improve sales predictions by leveraging clustering to account for store-specific patterns, such as outlet size, location type, and years of operation, while enhancing the performance of traditional machine learning models like Linear Regression, Ridge Regression, Random Forest, and XGBoost.

The **Clustering-Enhanced XGBoost** method integrates **k-means clustering** with regression models to segment stores into clusters based on shared characteristics. These clusters are then used as additional features in the model to capture store-specific sales patterns and improve predictive accuracy.

## **Codebase Overview**
The codebase consists of several key sections:

- **Data Preprocessing**: The dataset is loaded and cleaned, including handling missing values, encoding categorical variables, and engineering new features such as 'Years_Operating'.
  
- **Model Implementation**: Multiple models are implemented, including:
  - **Linear Regression**
  - **Ridge Regression**
  - **Random Forest Regressor**
  - **XGBoost** 
  - **Clustering-Enhanced XGBoost** (novel approach that integrates clustering into XGBoost)

- **Feature Engineering**: New features like **Years_Operating** are added, and categorical variables are encoded into dummy variables.

- **Clustering**: **k-means clustering** is used to group stores based on their attributes (e.g., Outlet Size, Location Type, Years Operating). The resulting **cluster labels** are then integrated into the XGBoost model.

- **Model Evaluation**: Each model is evaluated using standard metrics: **Mean Absolute Error (MAE)**, **Root Mean Squared Error (RMSE)**, and **R-squared (R2)**. The **Clustering-Enhanced XGBoost** model is compared to baseline models to assess performance improvement.

## **Setup Instructions**

### **1. Clone the Repository**
First, clone the repository to your local machine:

### **2. Follow along the notebook**

```bash
git clone https://github.com/yourusername/bigmart-sales-prediction.git
```

## **Evaluation Metrics**
The models are evaluated using the following metrics:
- **Mean Absolute Error (MAE)**: Measures the average absolute error between the predicted and actual sales values.
- **Root Mean Squared Error (RMSE)**: Gives more weight to larger errors, helping to understand model performance in extreme cases.
- **R-squared (R2)**: Indicates the proportion of variance explained by the model.

## **Contributing**
Feel free to fork the repository and submit pull requests for improvements or fixes. Please ensure that any contributions adhere to the existing coding standards and include necessary tests for new features.

