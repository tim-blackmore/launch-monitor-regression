# Udacity-Assignment-1
 
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
From the dataset, two variables were identified as the dependant variables, or the varaibles to be predicted (Total, Side Total). These data were also combined to create a third dependant variable labelled Distance-Accuracy.

2 varaibles (Impact Offset & Impact Width) were dropped as they contained too much missing data to be sensibly imputed. Data were assesed for univaraite outliers. These made up only a small proportion of the data and it was unlikely that they were due to measurement error so they were retained.


6. Modelling
7. Evaluation
8. Deployment
N/A.

## Acknowledgements
