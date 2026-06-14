# Digit_recoginzation 
##  Handwritten Digit Recognition using Neural Network (MNIST)
Project Overview

This project implements a simple Artificial Neural Network (ANN) using TensorFlow/Keras to classify handwritten digits (0–9) from the MNIST dataset.

The model takes 28×28 grayscale images as input, flattens them into a 1D vector, and predicts the digit using a fully connected neural network.

This project demonstrates the fundamentals of:

1.Deep Learning basics

2.Image preprocessing

3.Dense neural networks (ANN)

4.Model evaluation and prediction analysis

 Dataset:
 
1.Dataset: MNIST Handwritten Digits

Source: TensorFlow/Keras built-in dataset

60,000 training images

10,000 testing images

Image size: 28×28 pixels (grayscale)

 Model Architecture

Two ANN models were experimented:

1. Model 1 (Simple Logistic Regression Style NN)
Flatten input (28×28 → 784)
Dense layer (10 neurons, sigmoid activation)

2. Model 2 (Improved ANN)
Flatten input (784)
Dense layer (100 neurons, ReLU activation)
Dense layer (10 neurons, sigmoid activation)

Tech Stack :

Python 

TensorFlow / Keras

NumPy

Matplotlib

Seaborn

 Data Preprocessing
Normalized pixel values (0–255 → 0–1)

Flattened images from 2D (28×28) to 1D (784)

Used sparse categorical label 

Training Details

Optimizer: Adam

Loss Function: Sparse Categorical Crossentropy

Epochs: 5–10

Batch Size: Default (32)

 Model Performance
Model 1:

Test Accuracy: ~92–93%

Model 2:

Test Accuracy: ~97–98%

 Evaluation
Confusion Matrix

A confusion matrix was used to evaluate model predictions and understand classification errors across all digit classes.

Prediction Example

Model correctly predicts most digits

Some misclassifications observed between similar digits (e.g., 4 vs 9, 3 vs 5)

Key Insights

Increasing hidden neurons improves accuracy significantly

ReLU activation performs better than sigmoid in hidden layers

Flattening images is a simple but effective approach for ANN baseline

Model performs well but struggles with visually similar digits

 How to Run
1. Clone repository
git clone https://github.com/hansi1154/Digit_recoginzation.git

cd mnist-ann
3. Install dependencies
pip install -r requirements.txt
4. Run notebook


