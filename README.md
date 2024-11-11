# Predicting Student Loan Repayment with a TensorFlow Neural Network

This project uses a neural network model to predict whether a student loan borrower will repay their loan.

## Project overview

This project includes:

* A Keras model that predicts whether students will repay their student loan debt.

* Validation of the model's `accuracy` and `loss`.

* Output of the model to a .keras file in the `saved_models` folder so that we can easily retrieve it for use and validation.

* Retrieval of saved model
  
* Compilation, predictions, f1 score, and final analysis

## Model configuration

### Input layer

The number of features is defined by referencing the length of the `X_train` DataFrame. This comes out to `11` features based on the current training dataset.

### Hidden layers

There are two hidden layers.

* Layer 1: 6 nodes with `relu` activation.
* Layer 2: 3 nodes with `relu` activation.

### Output layer

1 node

### Compilation

```nn.compile(loss='binary_crossentropy', optimizer='adam', metrics=['accuracy'])```

## Model validation

```Current results - Loss: 0.5247386693954468, Accuracy 0.737500011920929```

## Predictions classification report

* f1 score: 0.74
* Weighted accuracy: 0.74
* Macro accuracy: 0.74
