# Hyperparameter Tuning with Keras on MNIST

## Overview

This project demonstrates the impact of hyperparameter tuning on the performance of a multi-layer perceptron (MLP) model using the MNIST dataset. Various techniques are applied, including weight initialization, activation functions, optimizers, batch normalization, and dropout regularization, to enhance the model's accuracy.

## Objectives

- To explore and implement various hyperparameter tuning techniques.
- To analyze the performance improvements on the MLP model.
- To achieve optimal accuracy on the MNIST dataset.

## Dataset

The MNIST dataset consists of 70,000 grayscale images of handwritten digits (0-9). The dataset is split into 60,000 training images and 10,000 test images.

## Installation

To run this project, ensure you have the following dependencies installed:

```bash
pip install numpy matplotlib keras
```

## Model Architecture

The MLP model consists of:

- **Input layer** (784 neurons)
- **Multiple hidden layers** with:
  - **Activation functions**: ELU, ReLU, and Sigmoid
  - **Weight initialization**: He Normal
  - **Regularization techniques**: Batch Normalization and Dropout
- **Output layer** (10 neurons for classification)

## Techniques Applied

- **Weight Initialization**: *He Normal* initialization to address the vanishing gradient problem.
- **Activation Functions**:
  - *Sigmoid*
  - *ReLU*
  - *ELU*
- **Optimizers**:
  - *Stochastic Gradient Descent (SGD)*
  - *Adam*
- **Regularization**:
  - *Dropout* (20% rate)
  - *Batch Normalization*

## Visualization

The training and validation accuracy are plotted for each configuration to visualize the model's performance over epochs. 

- **Training Accuracy**: The accuracy achieved by the model on the training dataset during training.
- **Validation Accuracy**: The accuracy achieved by the model on the validation dataset, indicating how well the model generalizes to unseen data.

The plots illustrate the effectiveness of various techniques implemented throughout the project, including:
- *Weight initialization methods*
- *Activation functions*
- *Regularization techniques*

## Results

- **Test Accuracy**:
  - *Initial naive MLP*: ~11.3%
  - *After implementing He Normal Initialization*: ~37.2%
  - *After using ReLU activation*: ~92.2%
  - *After applying Adam optimizer*: ~95.8%
  - *With Batch Normalization*: ~96.5%
  - *With Dropout Regularization*: ~88.9%

*Note: The above accuracies are based on various configurations applied throughout the project.*

