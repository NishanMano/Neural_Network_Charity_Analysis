# Neural_Network_Charity_Analysis
-----

# Overview: 
We are helping a non-profit foundation that wants to bring the world together through various means such as improving human's quality of life and assisting various environmental organizations. When we a company wishing to donate money to various platforms, we are bound to encounter a few bad apples (investments)! Therefore we will use our machine learning model to predict which organizations we should be donating towards and which organizations we should avoid. 

## Data: 
We use the data provided from Alphabet Soup's team, which provides a CSV file containing more than 34,000 organizations worldwide that Alphabet Soup has provided donations for throughout numerous years. Within this dataset are a number of columns that capture metadata about each organization.
 
- Target Model = IS_SUCCESSFUL

- Features of the model incldues all columns minus IS_SUCCESFUL EIN and 
 
  - APPLICATION_TYPE—Alphabet Soup application type

  - AFFILIATION—Affiliated sector of industry

  - CLASSIFICATION—Government organization classification

  - USE_CASE—Use case for funding

  - ORGANIZATION—Organization type

  - STATUS—Active status

  - INCOME_AMT—Income classification

  - SPECIAL_CONSIDERATIONS—Special consideration for application

  - ASK_AMT—Funding amount requested

- Not Targets nor Features:
  - EIN and NAME—Identification columns

## Data Cleaning: 
We drop a few columns in order to make our vast data, more concise and provide better accurate results when we run our machine learning model. We use a density plot to determine the distribution of the column values. The reason behind this image below is that if we have too many unique columns it will make our data less accurate. We would lump these unique columns in order to enhance our analysis. We used an application type which combines all types which are below 200: 

![1](https://i.ibb.co/wJSLvhb/1.png)

![2](https://i.ibb.co/LYbk6LG/2.png)

![3](https://i.ibb.co/BG57S9Q/3.png)

![4](https://i.ibb.co/QXwc0LX/4.png)

We finally scaled the data in order to remove any variability that may cause issues with our machine learning model.

## Model: 

After we preprocessed our data, we had a total of 34,299 rows and 44 columns as shown in the image below:

![5](https://i.ibb.co/tZWvSh2/5.png)


We then created a neural network model, by choosing the number of input features and nodes for each layer using Tensorflow Keras. We initially used 2 hidden layers and selected the relu actiovation function as well as the signmoid activation function. It is always best practice to check the structure of the model as shown in the image below: 

![6](https://i.ibb.co/y8C6qj8/6.png)

Model Optimization & Evaluation: 
Our target goal was to achieve a predictive accuarcy higher than 75% by using various methods to fine tune our model. 

Attempt #1: Adding One Additional Hidden Layer:
![5](https://i.ibb.co/yS3KkZZ/Attempt1.png)

Attempt #2: Adding Two Hidden Layers & Changing Activation Function: 
![6](https://i.ibb.co/Qp3gBVr/Attempt2.png)

Attempt #3: Adding Four Hidden Layers & Changing Activation Function: 
![7](https://i.ibb.co/wz9CwYr/Attempt3.png)




