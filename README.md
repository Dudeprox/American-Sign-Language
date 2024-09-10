# American Sign Language Classification - CSC413 Assignment 2

## Project Overview
This project focuses on classifying hand gestures representing the letters A-I in American Sign Language (ASL) using Convolutional Neural Networks (CNNs). The dataset consists of images of hand gestures taken by students, and the task involves building and training CNN models to predict the correct letter from a given image.

## Getting Started

### Prerequisites
- Python 3.x
- PyTorch
- Torchvision
- Google Colab (recommended)

### Dataset
Download the dataset from [Google Drive](https://drive.google.com/drive/folders/1aPL24P610NHLvt9exk6-B7SzGk3R8Q48?usp=sharing) and organize it as:
- `train/`: Training data
- `valid/`: Validation data
- `test/`: Test data

Ensure the data structure follows the format required by `torchvision.datasets.ImageFolder`.

### Model Architectures
- Model 1: Simple CNN without dropout/batch normalization.
- Model 2: CNN with batch normalization/dropout.
- Transfer Learning: Utilize pre-trained AlexNet for feature extraction.

### Training
- Models are trained using a PyTorch DataLoader with adjustable batch sizes and epochs.
- Hyperparameter tuning is performed to optimize learning rates and architectures.

### Evaluation
- Models are evaluated based on accuracy on validation and test datasets.
- Transfer learning using AlexNet significantly improves accuracy.

### Sanity Check
- Overfit the model on a small subset of data to verify the correctness of the training code.

### Additional Features
- Adversarial Examples: Generate adversarial noise to misclassify an image while keeping the noise imperceptible.