# Neural Network Regression Model for Predicting MEDV

This repository contains a Python script that implements a neural network regression model using Keras to predict the Median Value of owner-occupied homes (MEDV) based on the Boston Housing dataset. The model is trained, validated, and tested using a dataset loaded from a CSV file.

Dataset
# Dataset
The dataset used in this project is expected to be in a CSV file named `TP6_dataset.csv`. The dataset should contain the following features:

- **CRIM**: Per capita crime rate by town.
- **ZN**: Proportion of residential land zoned for lots over 25,000 sq.ft.
- **INDUS**: Proportion of non-retail business acres per town.
- **CHAS**: Charles River dummy variable (1 if tract bounds river; 0 otherwise).
- **NOX**: Nitric oxides concentration (parts per 10 million).
- **RM**: Average number of rooms per dwelling.
- **AGE**: Proportion of owner-occupied units built prior to 1940.
- **DIS**: Weighted distances to five Boston employment centers.
- **RAD**: Index of accessibility to radial highways.
- **TAX**: Full-value property tax rate per $10,000.
- **LSTAT**: Percentage of lower status of the population.
- **MEDV**: Median value of owner-occupied homes in $1000s (target variable).

# Model Architecture
The neural network model consists of the following layers:

- **Input Layer**: Dense layer with 64 units and ReLU activation.
- **Hidden Layer 1**: Dense layer with 32 units and ReLU activation.
- **Hidden Layer 2**: Dense layer with 16 units and ReLU activation.
- **Output Layer**: Dense layer with 1 unit (no activation function for regression).

# Training
The model is trained using the Adam optimizer and Mean Squared Error (MSE) as the loss function. The training process includes:

- **Training Set**: 70% of the data.
- **Validation Set**: 30% of the training data.
- **Test Set**: 20% of the original data.

The model is trained for 100 epochs with a batch size of 32.

# Evaluation
The model's performance is evaluated on the test set using the following metrics:

- Mean Absolute Error (MAE)
- Mean Squared Error (MSE)
- R-squared (R²)
