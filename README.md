# Neural_Network_Charity_Analysis

## Analysis Overview

Purpose of this analysis is to use deep-learning neural networks with tensor flow to analyze and classify the success of charitable donations.

Using the following methods for analysis: 
* preprocessing the data for the neural network model
* compile, train and evalusate the model
* optimize the model

## Results

### Data Preprocessing
* The column IS_SUCCESSFUL is the target variable for our deep learning network due to the data referint to weither or not the charity donation was used effectively
* The columns APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, SPECIAL_CONSIDERATIONS, ASK_AMT are the features for the model
* The columns EIN and NAME are identification information and are removed from the input data

### Compiling, Training, and Evaluating the Model
* The neural network model is made of two hidden layers with 80 and 30 neurons. The input data has 43 features and 25,724 samples. The output layer is made of a unique neuron as it is a binary classification. To speed up the training process, used activation function ReLU for the hidden layers and used Sigmoid on the output layer.
* The model accuracy came out to be under 75% which is an unsatisfactory performance to help predict the outcome of the charity donations.
* To increase the performance of the model, increased the number of neurons of the hidden layers, added another hidden layer, and tried a different activation function(tanh) but none of these steps helped improve the accuracy of the model.

## Summary

* The deep-learning neural network model did not reach the target of 75% accuracy. Since this target level is average we could say that the model is not outperforming.

* With it being a binary classification situation, could use a supervised machine learning model like Random Forest Classifier to combine a multitude fo decision trees to generate an outcome and evaluate its performance againts our neural network model.
