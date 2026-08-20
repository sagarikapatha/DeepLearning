# Deepfake Image Detection Using CNN

A computer vision project that classifies images as real or fake using a Convolutional Neural Network built with TensorFlow and Keras.

## Project Overview

This project explores deepfake image detection using a CNN-based binary classification model.

The workflow includes image preprocessing, dataset splitting, data augmentation, CNN model development, hyperparameter tuning, evaluation, and prediction visualization.

## Tech Stack

- Python
- TensorFlow
- Keras
- OpenCV
- NumPy
- Matplotlib
- Scikit-learn
- Keras Tuner

## Project Workflow

1. Loaded real and fake images using OpenCV
2. Resized images to 64 × 64 pixels
3. Converted images into NumPy arrays
4. Split data into training, validation, and test sets
5. Applied image normalization and augmentation
6. Built a CNN using Conv2D, MaxPooling, Dense, and Dropout layers
7. Used Keras Tuner RandomSearch for hyperparameter tuning
8. Trained the tuned CNN for 10 epochs
9. Evaluated the model on the test dataset
10. Visualized predictions for real and fake images

## Model Architecture

The tuned CNN includes:

- Conv2D layers
- MaxPooling2D layers
- Flatten layer
- Dense layer
- Dropout regularization
- Sigmoid output for binary classification

The tuned model contains approximately 11.3 million trainable parameters.

## Model Evaluation

Best validation accuracy during tuning: approximately **57.1%**

Final test accuracy: approximately **53.1%**

The results show that the model learned some distinguishing image patterns, but performance remains limited and provides opportunities for further improvement.

## Future Improvements

- Increase dataset size and diversity
- Use transfer learning with models such as EfficientNet or ResNet
- Improve class balancing
- Tune additional hyperparameters
- Add precision, recall, F1-score, and confusion matrix evaluation
- Experiment with higher image resolution
- Apply stronger regularization techniques

## Files

- `Deepfakes.ipynb` - complete model development and evaluation
- Project report
- Scientific paper
- Presentation materials
