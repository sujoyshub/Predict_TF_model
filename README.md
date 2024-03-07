# Predict_TF_model

The objective is to builds a simple Tensorflow model to predict if customer will churn based on a dummy customer data set.
These steps are basic and foundational steps when working with tensorflow.

>[!IMPORTANT]
> Here advance cases are not considerd like preprocessing (cleaning the dataset), plot performance metrices and also buliding model pipeline

The following sections are covered:

## 1.	Import Dependencies
```
# Sequential: Groups a linear stack of layers
# load_model: helps to reload model from memory later
# Dense Layer: regular densely-connected NN layer (hidden layers)
# accuracy_score: metric to evaluate how well the model is performing
```
## 2.	Build the model
```
# Instantiate the sequential class
# Add a bunch of layers to the NN, 2 hidden layers in this case
# units: x neurons inside of this dense layer
# activation: this function acts as a modifier to the o/p from NN
# relu activation: Takes the o/p and pass it through a function that will convert
# all negative values to zero and preserve all the positive values,
# converting this into a non-linear patterns making it powerful
# sigmoid activation: takes any o/p and converts it into a range between 0 & 1
```
## 3.	Compile the model
```
# Tell tensorflow, how to train the model
# What loss metrics and optimizer to be used and metric to focus on
# metrics to be evaluated by the model during training and testing
# SGD Optimizer: Gradient descent (with momentum) optimizer
```
## 4.	Fit, Predict and Evaluate
```
# FIT or train: pass X & y training dataframes
# epochs: specifies as how long to train for, higher epochs value may lead to overfitting
# batch_size: how large batch to be passed through tensorflow before an update is made

# PREDICTION: to be done on the X test dataframe
# TF result will be a continuous flow between 0.0 & 1.0. Hence convert this into a binary outcome of 0 or 1.

# EVALUATION: using accuracy score
```

## 5.	Save and Reload model
```
# save the model in the target folder specified
# delete model from memory
# reload model 
```

