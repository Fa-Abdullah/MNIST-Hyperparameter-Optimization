# MNIST Hyperparameter Tuning - Grid Search vs Random Search

A machine learning project that compares **Grid Search** and **Random Search** for hyperparameter optimization on the MNIST handwritten digit dataset using TensorFlow, SciKeras, and Scikit-learn.

---

## Overview

Selecting the right hyperparameters is essential for building high-performing machine learning models.

This project evaluates two popular hyperparameter optimization techniques:

- Grid Search
- Random Search

Both methods are applied to a Multi-Layer Perceptron (MLP) trained on the MNIST handwritten digit dataset, and their performance is compared based on cross-validation and test accuracy.

---

## Features

- MNIST handwritten digit classification
- Neural network built with TensorFlow/Keras
- Hyperparameter tuning using Grid Search
- Hyperparameter tuning using Random Search
- Cross-validation with SciKeras
- Performance comparison between both methods
- Final model evaluation on the test dataset

---

## Technologies Used

| Category | Technologies |
|----------|--------------|
| Programming Language | Python |
| Deep Learning | TensorFlow / Keras |
| Hyperparameter Optimization | Scikit-learn, SciKeras |
| Scientific Computing | NumPy, SciPy |
| Dataset | MNIST |

---

## Dataset

The project uses the **MNIST Handwritten Digits** dataset.

- 60,000 training images
- 10,000 testing images
- Image size: 28 × 28 pixels
- 10 digit classes (0–9)

Images are flattened into **784 input features** before training.

---

## Model Architecture

The neural network consists of:

- Input layer (784 features)
- Hidden layer with **64 ReLU neurons**
- Output layer with **10 Softmax neurons**

---

## Hyperparameters

The following parameters were optimized:

| Parameter | Grid Search | Random Search |
|----------|-------------|---------------|
| Learning Rate | 0.001, 0.01, 0.1 | Random values |
| Batch Size | 32, 64 | Random values |
| Epochs | 10 | Random values |

---

## Results

| Method | Cross Validation Score | Test Accuracy |
|--------|------------------------|---------------|
| Grid Search | **96.86%** | **97.25%** |
| Random Search | **95.86%** | — |

### Best Grid Search Parameters

- Learning Rate: **0.001**
- Batch Size: **32**
- Epochs: **10**

The optimized model achieved **97.25% accuracy** on the MNIST test set.

---

## Usage

Open the notebook and execute all cells.

The notebook will:

1. Load the MNIST dataset.
2. Build the neural network.
3. Perform Grid Search.
4. Perform Random Search.
5. Compare both optimization methods.
6. Train the best model.
7. Evaluate performance on the test dataset.

---

## Key Findings

- Grid Search achieved the highest cross-validation accuracy.
- A smaller learning rate (0.001) produced the best results.
- Batch size significantly affected model performance.
- Hyperparameter optimization improved overall model accuracy.
- Grid Search provided the most reliable configuration for this experiment.

---

## Author

**Fatma Abdullah**
This project is open source and intended for educational and research purposes.
````
