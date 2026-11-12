# Arabic Handwritten Digit Recognition using PyTorch

A university assignment developed for **CPCS-432: Artificial Intelligence 2** at King Abdulaziz University.

This project implements a fully connected Artificial Neural Network (ANN) using PyTorch to classify handwritten Arabic digits from the AHDD dataset.

## Dataset & Model

- **Dataset:** AHDD - 60,000 training images and 10,000 test images (28 x 28 pixels).
- **Preprocessing:** Pixel normalization to [0, 1] and conversion to PyTorch tensors.
- **Architecture:** 784 input features, 128 hidden neurons (ReLU), and 2 or 10 output classes.
- **Training:** SGD optimizer, CrossEntropyLoss, 20 epochs, and batch size of 128.

## Experiments

The assignment explored:

- Binary classification of digits 6 and 7 versus classification of all ten digits (0-9).
- Three learning rates: 0.001, 0.01, and 0.1.
- Three random seeds: 1, 10, and 42.

## Key Results

| Classification | Baseline Accuracy (LR = 0.01) | Best Accuracy (LR = 0.1) |
|---|---|---|
| Two-class (6 and 7) | 99.65% | **99.95%** |
| Ten-class (0-9) | 95.72% | **97.54%** |

The learning rate of 0.1 achieved the highest accuracy among the tested values. Changing random seeds produced only small differences in accuracy.

## Technologies

Python, PyTorch, Artificial Neural Networks, Image Classification

## Notebook

See [arabic_digit_recognition_ann.ipynb](https://github.com/iMur4d/arabic-handwritten-digit-recognition/blob/main/arabic_digit_recognition_ann.ipynb) for the implementation, training experiments, and evaluation results.
