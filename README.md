# SC1015-MiniProject
School of Computer Science and Engineering

Nanyang Technological University

Lab: C133 Group : 9

Members: 
  
  Dexter Ng
  
  Sruthi Sathishkumar
  
  Yen Zhi Wei 
  
# Description 

This repository contains  the Jupyter Notebook and dataset we use to create the mini project. This README file highlights what we have done for this project. Detailed information will be available in the notebook. 

# Table of content
 #### 1. Problem Formulation  
 #### 2. Data Preparation and Cleaning
 #### 3. Exploratory Data Analysis
 #### 4. Regression Models
 #### 5. Conclusion 
# 1. Problem Formulation 
Our dataset: https://api.covidtracking.com/v1/us/daily.csv from The COVID Tracking Project

Our Problem Statement: Which regression model can best predict the number of COVID-19 hospital admissions based on predictor variables?
 
We chose to do Covid-19 because even though the world is slowly recovering from the aftermaths of the pandemic, we believe that we should not be complacent and instead remain vigilant in tackling the pandemic. With strains on global healthcare systems and limitations in facilities, by doing an analysis on the dataset, we can find out what are the main factors that can predict the number of hospital admissions to the hospital. By learning which model is the best suited for this case study, we can make use of the skills and models learnt to apply in other similar/potential areas (e.g. another virus)
and better understand what it takes to predict the hospitalisation rates. 



# 2. Data Preparation and Cleaning
With the dataset we choose, it is not 100% useful and needs to be cleaned to our desired outcome for the most optimal result. 

We did the followig: 

1. Specific Selection: Out of 25 variables, 6 variables were used.
2. Dropping of NaN values: Variables with NaN values were dropped (e.g. "recovered")
3. Changing of Date Format: Given format was 20210307. We changed using  format='%Y%m%d'  for graph accuracy. 

# 3. Exploratory Data Analysis & Visualization
For Visualization we used Plotly. Plotly has interactive visualiztion, wide range of charts, and it is simple to implement.
With the aid of the chart, we were then able to spot trends and pattern from the different variables we selected (e.g. As the month increases, number of negative cases also increases)
We also plot the predictor varibles and response variable. Information such as median, min and max were available for analysis. 

For more information and better understanding, please refer to our notebook. 
# 4. Regression Models
Before we start, we had to split our data into train and test. We split it into 80:20 ratio and choose random state 1 to ensure 
the same train and test sets across different executions. For model accuracy indicator, we used Explained Variance (R^2). It is a measure of prediction accuracy,
it is the variance between actual & predicted values, the higher the R^2 value, the better the model

1. Linear Regression Model: used to analyze the relationship between a dependent variable and one or more independent variables.
2. Polynomial Regression Model: models the relationship between the independent variable and the dependent variable as an nth degree polynomial equation. 

More details of the regression models are preseted in our notebook. 
# 5. Conclusion
After analysis of the two regression model and finding the R^2 value, we can then determine which regression model is the better one. Linear Regression was the 
better one since it has the highest R^2 value as comapared to Polynomial Regression. The findings have been presented in the  Notebook.

Through this Mini-Project, our group has learnt many new functions and new regression model. We now better understand data preparation and how to analysis data with 
the different function available. 

Thank you. 

References
- https://covidtracking.com/
- https://covidtracking.com/data/api
- https://covid19.who.int/
- https://jamanetwork.com/journals/jamanetworkopen/fullarticle/2789848
