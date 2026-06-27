# MNIST Hyperparameter Tuning - Grid Search vs Random Search

A comparative study of Grid Search and Random Search for hyperparameter optimization on MNIST dataset using scikeras and scikit-learn.

## Overview

This project demonstrates hyperparameter tuning techniques on a simple neural network trained on MNIST:
- **Grid Search**: Exhaustive search over predefined parameter grid
- **Random Search**: Randomized search over parameter distributions

## Dataset

- **MNIST**: 60,000 training images, 10,000 test images
- 28x28 grayscale images of handwritten digits (0-9)
- Flattened to 784 features

## Model Architecture

```python
Sequential([
    Dense(64, activation='relu', input_dim=784),
    Dense(10, activation='softmax')
])
