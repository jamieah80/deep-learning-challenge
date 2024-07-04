## Report on Neural Network Model
Module 21 Challenge - UoB Data Analytics Bootcamp

## Overview
This project looked to analyse if funding given to charities was used successfully. A model would be trained to advise regarding future applications for funding.

## Results
# Data Preprocessing
    -  The target for the model is the "IS_SUCCESSFUL" column, the indicator whether the funcing was used successfully.
    -  The variables used in this model were APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, SPECIAL_CONSIDERATIONS, ASK_AMT
    - The STATUS and SPECIAL_CONSIDERATIONS columns could be dropped due to all values being the same.

# Compiling, Training, and Evaluating the Model
    - In the first model, only two hidden layers were used, both with "relu" activation function. In the optimised code, this was increased to four hidden layers, with two new hidden layers using the "sigmoid" activation function. The use of the additional layers increased accuracy.
    -Ultimately this did not meet the target of 75%, despite multiple attempts with a variety of combinations of activation functions and layers.

## Summary

Whilst we did not reach 75%, we did achieve 74% accuracy, which means applications would be correctly classified 74% of the time.

For future models, a random forest may be more appropriate. This is commonly utilised for classification problems such as this, where a decision tree can be created from the training data. It can also scale to suit this use.
