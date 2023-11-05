# Image Classification with TensorFlow and Keras

This repository contains code for organizing a gesture dataset and training an image classification model using TensorFlow and Keras. The dataset is organized into class-based folders, and a Convolutional Neural Network (CNN) model is trained to classify the gestures. The trained model is then tested on new images.

## Dataset Organization

The `GestureDatasetOrganizer` file organizes the dataset. It assumes you have a source folder `leapGestRecog` with subfolders containing image data. The code organizes them into class-based folders inside the "Data" directory.

## Model Training

The `Train` file trains an image classification model using TensorFlow and Keras. The steps include:

1. Loading and splitting the dataset into training and validation sets.
2. Creating a CNN model using Keras' Sequential API.
3. Compiling the model with an optimizer, loss function, and metrics.
4. Training the model on the training dataset and validating it on the validation dataset.
5. Saving the trained model to a file.

## Model Testing

The `Test` file tests the trained model with new images. It randomly selects one image from each class subfolder in the "Data" directory and copies it to the "Test Data" directory. It then loads the pre-trained image classification model and tests it on the new images.

## Prerequisites

- Python 3.x
- TensorFlow
- Keras
- Matplotlib
- PIL (Python Imaging Library)
- NumPy

## Usage

1. Organize your dataset using the `GestureDatasetOrganizer` file.
2. Train the model using the `Train` file.
3. Test the model using the `Test` file.


