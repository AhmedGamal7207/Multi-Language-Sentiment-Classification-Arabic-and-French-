# Multi-Language Sentiment Classification (Arabic and French)

## Overview
This repository contains sentiment classification models for Arabic and French using deep learning. The models leverage Recurrent Neural Networks (RNNs) with Long Short-Term Memory (LSTM) layers to classify sentiment as either positive or negative. The project includes data preprocessing, model training, and evaluation for both languages.

## Dataset

1. **Egyptian Arabic Dataset**: A dataset containing Egyptian Arabic sentences labeled as positive or negative.
2. **French Dataset**: A dataset containing French sentences labeled as positive or negative.

## Preprocessing

The following steps are used for both datasets:

- **Tokenization**: Sentences are tokenized, with unknown words replaced by `<OOV>`.
- **Padding**: Sequences are padded to ensure uniform input length.
- **Splitting**: The data is split into training and test sets (80/20).

## Model Architecture

### 1. **RNN with LSTM**
- **Embedding Layer**: Each word is represented as a 16-dimensional vector.
- **LSTM Layer**: Used for learning the sequential patterns in the data.
- **Dense Layer**: Final output layer for binary classification (positive/negative).
- **Activation Function**: Sigmoid activation function for classification.

### 2. **Optimizers and Loss Functions**
- **Optimizer**: Adam optimizer is used.
- **Loss Function**: Binary Cross-Entropy is used for binary classification.

## Training and Evaluation

Both models were trained for 8 epochs with early stopping to avoid overfitting. The evaluation is based on the test accuracy for each language:

- **Arabic Sentiment Model**: Achieved 91.34% accuracy on the test set.
- **French Sentiment Model**: Achieved 70.75% accuracy on the test set.

## Example Usage

You can use the models to predict sentiment from input sentences.

