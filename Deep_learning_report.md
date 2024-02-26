# Module 21 Report 

## Overview of the Analysis

## Purpose

The purpose is to create a binary classifier that can predict the success of the organizations if funded by the fictional non-profit foundation , Alphabet Soup.

## process 

*The preprocessing start with removing irrelevent variabiles , Name and EIN.  

*The target variable is "IS_SUCCESSFUL". 

*The remaining columns are used as the features of the model.

*APPLICATION_TYPE AND CLASSIFICATIONS columns used for binning to lower the unique values to less than 10. 

*The categorical data is then converted to numerical using `pd.get_dummies()`

*`Train_test_split` applied to create testing and training data and then scaled with `StandardScaler`

## Compiling, Training, and Evaluating the Model

Create a neural network model by assigning the number of input features and nodes for each layer using TensorFlow and Keras.

Create the first hidden layer and choose an appropriate activation function.

Add hidden layers with an appropriate activation function.

Create an output layer with an appropriate activation function.

Check the structure of the model.

Compile and train the model.

The first model :
    Application Type cut off = 500
    classification Cutoff = 500
    Hidden layer 1 : nodes= 80 Actication function = Relu
    Hidden layer 2 : nodes = 30 Actication function = Relu
    
First attempt for optimization :
    Application Type cut off = 800
    classification Cutoff = 1000
    Hidden layer 1 : nodes= 80 Actication function = Relu
    Hidden layer 2 : nodes = 30 Actication function = Relu
    Hidden layer 2 : nodes = 20 Actication function = Relu

second attempt for optimization :
    Application Type cut off = 800
    classification Cutoff = 1000
    Hidden layer 1 : nodes= 80 Actication function = Relu
    Hidden layer 2 : nodes = 40 Actication function = Tanh
    Hidden layer 2 : nodes = 20 Actication function = Relu

Third attempt for optimization :
    Application Type cut off = 1000
    classification Cutoff = 500
    Hidden layer 1 : nodes= 90 Actication function = Relu
    Hidden layer 2 : nodes = 50 Actication function = Tanh
    Hidden layer 2 : nodes = 35 Actication function = Relu

## Results
The first model :
    Accuracy: 73.08
    Loss: 55.74
First attempt for optimization :
    Accuracy: 72.71
    Loss: 56.55

Second attempt for optimization :
    Accuracy: 72.76
    Loss: 55.86
  
Third attempt for optimization :
    Accuracy: 72.76
    Loss: 55.76
  
  
## Summary
The goal is to crate a model tp predict the success with more than 75% accuracy. The maximum accuracy tht could be achieved was only 73.08%. THis model need to be improved by adiitional cleaning of data and using different model for deep learning to improve the accuracy of the prediction.


