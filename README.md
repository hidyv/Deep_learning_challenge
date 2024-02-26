# deep_learning_challenge

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

## Summary

The goal is to crate a model tp predict the success with more than 75% accuracy. The maximum accuracy tht could be achieved was only 73.08%. THis model need to be improved by adiitional cleaning of data and using different model for deep learning to improve the accuracy of the prediction.