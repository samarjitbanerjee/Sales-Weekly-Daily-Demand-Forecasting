# Sales-Weekly-Daily-Demand-Forecasting
Problem Statement - 

There are large warehouses where products are reaching and these products are distributed among short warehouses/Distributors.The Weekly Dispatch count is measured on Sunday alone and through out the week, daily dispatch count is measured. Objective is to build a demand forecasting model to forecast for weekly & daily sales of products.

Objective:
Predict Weekly & Daily Dispatch Count

DataSet:
Along with Independent Varibales like, day of week, day, is_weekend there are two target variables(One refers to Daily Dispatch count and other one to weekly dispatch count)

KPI:
MAPE(Mean Absolute Perecentage Error) - max(0,100*(1-(mean_absolute_percentage_error(y_true,y_pred))))

Data Cleaning/Analysis/Preparation
1. Missing Values Impuation - is_warehouse_closed, Latitude,Longitude Replacing NAN values of weekly dispatch with the corressponding week's weekly dispatch count measured on Sunday
2. Feature Engineering
3.Encoding Features.

Model Training:
1. Random- Train Test Split.
2. Model-1: Predict Weekly Dispatch Count(Deep Neural Network - Considered Best Model)
   Model - 2: Predict Daily Dispatch Count(Deep Neural Network - Considered Best Model)
3. Define Custom Ensemble to invoke Model-1 and Model-2 to predict Weekly and Daily Dispatch Count
