# MNIST Handwritten Digit Classification using ANN

## Project Overview

This project focuses on classifying handwritten digits (0–9) using an Artificial Neural Network (ANN).

The model is developed using TensorFlow and Keras and trained on the MNIST dataset, which contains 70,000 grayscale images of handwritten digits.

The objective is to build a neural network that can accurately recognize handwritten digits from image data.

## Dataset

The project uses the **MNIST Handwritten Digit Dataset**, available through `keras.datasets`.

- Total Images: 70,000
- Training Images: 60,000
- Testing Images: 10,000
- Image Dimensions: 28 × 28 pixels
- Color: Grayscale
- Number of Classes: 10 (Digits 0–9)

Each image contains a handwritten digit represented by pixel intensity values ranging from 0 to 255.

## Technologies and Libraries

- Python
- NumPy
- Matplotlib
- Seaborn
- TensorFlow
- Keras
- Scikit-learn
- Pillow (PIL)

## Project Workflow

1. Importing required libraries
2. Loading the MNIST dataset
3. Inspecting dataset dimensions and labels
4. Visualizing sample handwritten digits
5. Analyzing class distribution
6. Normalizing pixel values
7. Building the ANN model
8. Training and validating the model
9. Visualizing training and validation performance
10. Evaluating the model on test data
11. Generating digit predictions
12. Analyzing the confusion matrix
13. Evaluating classification metrics
14. Predicting custom handwritten digit images

## ANN Architecture

The Artificial Neural Network consists of the following layers:

| Layer | Configuration |
|---|---|
| Input | 28 × 28 pixels |
| Flatten | Converts image into 784 features |
| Hidden Layer | 50 neurons, ReLU activation |
| Output Layer | 10 neurons, Softmax activation |

**Model Configuration:**

- Optimizer: Adam
- Loss Function: Sparse Categorical Crossentropy
- Evaluation Metric: Accuracy
- Epochs: 10
- Batch Size: 32
- Validation Split: 10%

## Model Performance

The model achieved the following results:

| Metric | Result |
|---|---:|
| Training Accuracy | 99.02% |
| Validation Accuracy | 97.32% |
| Test Accuracy | 97.11% |
| Test Loss | 0.1012 |
| Macro F1-score | 97.09% |
| Weighted F1-score | 97.11% |

The model was evaluated using a separate test dataset containing 10,000 images.

## Custom Image Prediction

The project also includes functionality to predict digits from custom handwritten images.

The uploaded image is converted to grayscale, inverted when necessary, cropped, resized, normalized, and transformed into the required 28 × 28 input format before prediction.

Prediction performance on custom images may vary depending on handwriting style and image quality.


## Conclusion

This project demonstrates how an Artificial Neural Network can be used for handwritten digit classification.

The model achieved 97.11% test accuracy on the MNIST dataset, demonstrating its ability to recognize handwritten digits with high accuracy.
