## Surprise Housing house pricing determination assignment
> The aim of the project is to build a regularised linear regression model for the prediction of hpuse prices in the Australian market for a US based company named Surprise Housing as they plan to venture into a new geography. The goal is to find the below:

- Which variables are significant in predicting the price of houses in the Australian market.
- How well those variables describe the price distribution of the houses in Australian market.


## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Steps Performed](#steps-performed)
* [Conclusions](#conclusions)



## General Information
- The project aims to achieve the identification of driving variables and their significance in predicting the prices of houses in Australian market.
- The project is a part of the curriculum of upGrad's IIIT Bangalore EPGP in Machine Learning and Artificial Intelligence.
- The business objective is to predict the price of the houses in Australian market.
- For analysis house pricing dataset from Surprise Housing has been taken for the houses sold in the years ranging from 2006 to 2010.



## Steps Performed
- Importing the necessary libraries
- Importing the dataset
- Exploratory Data Analysis
- Model creation using:
    1. Model 1 using statsmodels.api library
    2. Model 2 using Ridge model from scikit learn library.
    3. Model 3 using Lasso model from scikit learn library.
    4. Final model using RFE with Lasso estimator



## Conclusions
- From residual analysis for all the three models the conclusion is that multiple linear regression model is suitable for the dataset as the residuals do follow the assumptions of homoscedasticity and the residuals also follow a normal distribution. Also a linear relationship exists between the dependent variable and the predictor/independent variables.
- Out of the three models Lasso model is the best as it helps with 2 aspects:
    - Penalizing the parameters 
    - Feature Selection 
- When Lasso is combined with RFE we get a model which has less features but the test accuracy is still good. 
- Three top features were:
    1. GrLivArea
    2. OverallQual
    3. TotalBsmtSF
- Final model:
    𝑆𝑎𝑙𝑒𝑃𝑟𝑖𝑐𝑒=0.2794×𝑂𝑣𝑒𝑟𝑎𝑙𝑙𝑄𝑢𝑎𝑙+0.2385×𝑇𝑜𝑡𝑎𝑙𝐵𝑠𝑚𝑡𝑆𝐹+0.4091×𝐺𝑟𝐿𝑖𝑣𝐴𝑟𝑒𝑎−0.1053×𝐵𝑒𝑑𝑟𝑜𝑜𝑚𝐴𝑏𝑣𝐺𝑟+0.1480×𝐺𝑎𝑟𝑎𝑔𝑒𝐴𝑟𝑒𝑎−0.1955×𝐴𝑔𝑒𝑆𝑒𝑙𝑙𝑖𝑛𝑔+0.0835×𝐴𝑔𝑒𝑅𝑒𝑚𝑜𝑑𝑒𝑙𝑙𝑖𝑛𝑔+0.0775×𝑁𝑒𝑖𝑔ℎ𝑏𝑜𝑟ℎ𝑜𝑜𝑑𝐶𝑟𝑎𝑤𝑓𝑜𝑟+0.0736×𝑁𝑒𝑖𝑔ℎ𝑏𝑜𝑟ℎ𝑜𝑜𝑑𝑁𝑟𝑖𝑑𝑔𝐻𝑡+0.0865×ExteriorMat_Stucco & CmentBd+0.4439



## Technologies Used
- numpy - version 1.24.3
- pandas - version 1.5.3
- matplotlib - version 3.7.1
- seaborn - version 0.12.2
- statsmodels.ap1 - version 0.14.0
- sklearn - version 1.3.0



## Contact
Created by [@alokabhayajith] - feel free to contact me!