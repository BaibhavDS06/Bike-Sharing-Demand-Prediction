Bike Sharing Demand Prediction Project
Overview
This project aims to predict the demand for bike sharing services using historical data. The key steps include data cleaning, exploratory data analysis (EDA), hypothesis testing, model building, and deployment of a prediction application. The project leverages various machine learning models and Azure services for data pipeline management and deployment.
Key Steps
1. Data Cleaning
Objective: Ensure the data is free from inconsistencies and missing values.
Actions:
Handle missing values by imputation or removal.
Correct data types and formats.
Remove duplicates.
2. Exploratory Data Analysis (EDA)
Objective: Understand the data distribution and relationships between variables.
Actions:
Visualize data using histograms, scatter plots, and box plots.
Calculate summary statistics.
Identify key features influencing bike sharing demand.
3. Hypothesis Testing
Objective: Validate assumptions about the data.
Actions:
Formulate hypotheses (e.g., higher temperatures increase bike demand).
Perform statistical tests (e.g., t-tests, chi-square tests).
4. Dealing with Outliers and Multicollinearity
Objective: Improve model robustness by addressing data anomalies.
Actions:
Detect outliers using z-scores or IQR.
Remove or cap outliers.
Check for multicollinearity using VIF (Variance Inflation Factor).
Remove or combine highly correlated features.
5. Model Building
Objective: Develop predictive models to forecast bike sharing demand.
Models:
Linear Regression: Baseline model.
Regularization (Ridge, Lasso): Handle multicollinearity.
Decision Tree: Capture non-linear relationships.
Random Forest: Ensemble method for improved accuracy.
6. Model Tuning
Objective: Optimize model performance.
Actions:
Use Grid Search CV for hyperparameter tuning.
Evaluate models using cross-validation.
Select the best model (Random Forest achieved 90% accuracy).
7. Building ETL Pipeline in Azure Data Factory (ADF)
Objective: Fetch and preprocess live weather data.
Actions:
Set up data sources (e.g., weather API).
Create data pipelines for data extraction, transformation, and loading.
Schedule pipeline runs.
8. Building FastAPI-Based Prediction App
Objective: Develop a RESTful API for real-time predictions.
Actions:
Implement FastAPI endpoints for prediction.
Integrate with the trained model.
Test API using sample requests.
9. Docker File for Containerization
Objective: Package the prediction app for deployment.
Actions:
Create a Dockerfile to containerize the FastAPI app.
Build and test the Docker image locally.
10. Deployment Using Azure Container Registry (ACR) and Azure App Services
Objective: Deploy the prediction app to a scalable environment.
Actions:
Push the Docker image to Azure Container Registry.
Deploy the app using Azure App Services.
Configure environment variables and scale settings.
