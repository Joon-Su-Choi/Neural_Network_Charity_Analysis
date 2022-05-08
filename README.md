# Neural_Network_Charity_Analysis

## Overview of the Analysis

Through machine learning and neural networks we will help a nonprofit orgainization, Alphabet Soup, predict where to make investments. we will use the features in the provided dataset to create a binary classifier that is capable of predicting whether applicants will be successful if funded by Alphabet Soup. We received a CSV containing more than 34,000 organizations that have received funding from Alphabet Soup over the years. Within this dataset are a number of columns that capture metadata about each organization, such as the following:

- EIN and NAME—Identification columns
- APPLICATION_TYPE—Alphabet Soup application type
- AFFILIATION—Affiliated sector of industry
- CLASSIFICATION—Government organization classification
- USE_CASE—Use case for funding
- ORGANIZATION—Organization type
- STATUS—Active status
- INCOME_AMT—Income classification
- SPECIAL_CONSIDERATIONS—Special consideration for application
- ASK_AMT—Funding amount requested
- IS_SUCCESSFUL—Was the money used effectively

Our goal is the following:

- Preprocess the data for a neural network model.
- Compile, Train, and Evaluate the Model.
- Optimize the Model.

## Results

- Data Preprocessing
  - The variable we consider as the target for our model is the ```IS_SUCCESSFUL``` column.
  - The variables we consider as the features of our model are the following: ```APPLICATION_TYPE```, ```AFFILIATION```, ```CLASSIFICATION```, ```USE_CASE```, ```ORGANIZATION```, ```STATUS```, ```INCOME_AMT```, ```SPECIAL_CONSIDERATIONS```, and ```ASK_AMT```.
  - The variables that are neither targets nor features and that were removed from the input data were the ```EIN``` and ```NAME```.

- Compiling, Training, and Evaluating the Model
  -  There were two hidden layers, first layer containing 80 neurons and the second containing 30 neurons. The output layer is made of a unique neuron as it is a binary classification. We are using the activation function ReLU for the hidden layers. As our output is a binary classification, Sigmoid is used on the output layer. For the compilation, the optimizer is adam and the loss function is binary_crossentropy.
  - We did not achieve the target model performance as the model accuracy was under 75%.
What steps did you take to try and increase model performance?
  - To increase the model performance we did three attempts where he changed the amount of layers, neurons, and the activation functions. Despite our efforts, none of these steps improved the model's performance.

## Summary

Overall our results did not yield a target accuracy of 75% or higher. We can observe that our model is not outperforming. Since we are in a binary classification situation, we could use a supervised machine learning model such as the Random Forest Classifier to combine a multitude of decision trees to generate a classified output and evaluate its performance against our deep learning model.
