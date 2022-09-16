# Neural_Network_Charity_Analysis
-----

# Overview: 
We are helping a non-profit foundation that wants to bring the world together through various means such as improving human's quality of life and assisting various environmental organizations. When we a company wishing to donate money to various platforms, we are bound to encounter a few bad apples (investments)! Therefore we will use our machine learning model to predict which organizations we should be donating towards and which organizations we should avoid. 

## Data: 
We use the data provided from Alphabet Soup's team, which provides a CSV file containing more than 34,000 organizations worldwide that Alphabet Soup has provided donations for throughout numerous years. Within this dataset are a number of columns that capture metadata about each organization, such as the following:

EIN and NAME—Identification columns
APPLICATION_TYPE—Alphabet Soup application type
AFFILIATION—Affiliated sector of industry
CLASSIFICATION—Government organization classification
USE_CASE—Use case for funding
ORGANIZATION—Organization type
STATUS—Active status
INCOME_AMT—Income classification
SPECIAL_CONSIDERATIONS—Special consideration for application
ASK_AMT—Funding amount requested
IS_SUCCESSFUL—Was the money used effectively

## Data Cleaning: 
We drop a few columns in order to make our vast data, more concise and provide better accurate results when we run our machine learning model. We use a density plot to determine the distribution of the column values. The reason behind this image below is that if we have too many unique columns it will make our data less accurate. We would lump these unique columns in order to enhance our analysis. We used an application type which combines all types which are below 200: 

![1](https://i.ibb.co/wJSLvhb/1.png)

![2](https://i.ibb.co/LYbk6LG/2.png)

![3](

![4]( 

We finally scaled the data in order to remove any variability that may cause issues with our machine learning model.

## Model: 

After we preprocessed our data, we had a total of 34,299 rows and 44 columns as shown in the image below:

![5](


We then created a neural network model, by choosing the number of input features and nodes for each layer using Tensorflow Keras. We initially used 2 hidden layers and selected the relu actiovation function as well as the signmoid activation function. It is always best practice to check the structure of the model as shown in the image below: 

![6](
