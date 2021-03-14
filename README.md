# launch-monitor-regression

## Blog article
https://timblackmore.medium.com/smash-factor-not-heard-of-it-listen-up-942d25f92019

 
## Installation

The libraries used in this project are outlined in requirements.txt. They can be installed using the following command.

```pip3 install -r requirements.txt```

## Motivation

This project fulfils one of the requirements for the completion of the Data Science nanodegree with Udacity. 

## Project files

- requirements.txt - Contains the required packages to set up the development envrironment.
- data.csv - ~10000 rows. Data collected from a Trackman Launch Monitor which gives numeeric data on both golf club position and ball flight trajectory.
- main.ipynb - A jupyter notebook which contains the project code.

## Project summary

### 1. Business understanding
The goal is to complete the Data Science project as part of the Udacity nanodegree. 

We are free to choose the data source, but are required to create 3 questions that we address from the data. Success is defined as a completed jupyter notebook addressing the 3 questions as well as a blog post on Medium for non-technical stakeholders.

### 2. Data understanding
Data were collected from a Trackman Launch Monitor which gives numeeric data on both golf club position and ball flight trajectory. The data is entirely numeric but had to be converted to this format once imported. There are ~10000 rows. A correlation matrix and biplot was created to examine the relationship between the variables.

### 3. Data preparation
From the dataset, two variables were identified as the dependant variables, or the variables to be predicted (Total, Side Total). These data were also combined to create a third dependant variable labelled Distance-Accuracy.

Two variables (Impact Offset & Impact Width) were dropped as they contained too much missing data to be sensibly imputed. Data were assesed for univariate outliers. These made up only a small proportion of the data and it was unlikely that they were due to measurement error so they were retained.

### 4. Modelling
Linear regression was chosen to examine the relationship between the dependant and independant variables. Data were split into testing a training datasets. 3 models were created to assess 3 questions.

1. Which variables are predictive of driving distance - r2 score 0.86
2. Which variables are predictive of driving accuracy - r2 score 0.63
3. Which variables are predictive of a distance-accuracy tradeoff - r2 score 0.76

The goal was to determine which model coefficinets were mostly responsible for predicting the dependant variables. This was acheived via inspection of the model coefficients.

### 5. Evaluation
Models 1 and 3 performed well. All models could be improved with the creation of principal components or a stepwise appraoch to retaining/removing variables in order to make the model more parsimonious. But, as the goal was intepretation of which variables were most important via inspection of the model coefficients this was not possible. 

### 6. Deployment
N/A.

## Acknowledgements
Some functions relating to the linear regression were taken from the Udacity training materials.
