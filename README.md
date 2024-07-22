# COVID-19 Detection from Lung X-ray using CNN

This repository contains an implementation of a Convolutional Neural Network (CNN) model for binary classification to detect pneumonia from lung X-ray images. The model is trained using TensorFlow 2.0 and is part of a project to detect COVID-19 from medical imaging data.

## Dataset

The dataset used for training and evaluation is available on Kaggle:
- [COVID-19 X-ray Dataset (Train/Test Sets)](https://www.kaggle.com/datasets/khoongweihao/covid19-xray-dataset-train-test-sets)

The dataset includes X-ray images of lungs categorized into normal and pneumonia cases.

## Model Architecture

The CNN model implemented consists of several convolutional and pooling layers, followed by fully connected layers. The model architecture is designed to learn discriminative features from the X-ray images to classify them as either normal or pneumonia.

## Training

The model is trained using the TensorFlow 2.0 framework with the following configuration:
- Loss Function: Binary Crossentropy
- Optimizer: Adam
- Metrics: Accuracy

During training, early stopping and learning rate reduction on plateau callbacks are employed to monitor validation loss and prevent overfitting.

## Evaluation

The trained model's performance is evaluated on a separate test set from the dataset. Evaluation metrics such as accuracy and possibly precision, recall, and F1-score are computed to assess the model's effectiveness in detecting pneumonia from X-ray images.
