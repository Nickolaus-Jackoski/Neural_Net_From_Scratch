# Neural Network From Scratch

This project demonstrates the construction and training of a fully functional neural network **from scratch** using only Python and NumPy (no deep learning libraries like TensorFlow or PyTorch). It performs **binary classification** on a synthetic 2D dataset and explores how depth and architecture affect learning performance.

## Overview

- Implements a neural network class that supports:
  - Arbitrary number of layers
  - Arbitrary number of neurons per layer
  - Custom forward and backward propagation
  - Training with gradient descent
- Evaluates classification performance and visualizes decision boundaries
- Experiments with 1-layer, 2-layer, and 3-layer architectures

## Dataset

The dataset consists of 400 two-dimensional points split evenly into:
- 200 training samples
- 200 testing samples

Labels indicate class membership (`0` or `1`). Points are visually separable with nonlinear boundaries.

## Features & Functionality

- `NeuralNet` class implementation
  - Activation: ReLU (hidden layers), Sigmoid (output)
  - Loss: Cross-entropy
  - Training: Batch gradient descent
- Accuracy tracking and cost plotting
- Decision boundary visualization with Matplotlib
- Custom testing on 1-layer, 2-layer, and 3-layer neural networks

## Neural Architectures

- **1-layer network**: `2 → 1`
  - Baseline model; limited performance (≈50% accuracy)
- **2-layer network**: `2 → 4 → 1`
  - Achieves high accuracy (≈96.5% test accuracy)
- **3-layer network**: `2 → 3 → 3 → 1`
  - Demonstrates extensibility of the implementation

## Results

| Architecture | Train Accuracy | Test Accuracy |
|--------------|----------------|---------------|
| 1-layer      | ~52.5%         | ~52.5%        |
| 2-layer      | 100%           | ~96.5%        |
| 3-layer      | ~96.5%         | ~95.5%        |

## Files

- `output.csv` – Synthetic 2D dataset with labels
- `neural_net.ipynb` – Full implementation and analysis notebook

---

**Author:** Nickolaus Jackoski  
**Date:** June 4, 2025
