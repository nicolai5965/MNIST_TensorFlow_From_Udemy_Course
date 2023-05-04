# MNIST_TensorFlow_From_Udemy_Course
This is a ML model done one the MNIST dataset in TensorFlow. I have followed that Udemy course "the-data-science-course-complete-data-science-bootcamp" and then done some smalle changes my self.

This repository contains a TensorFlow implementation of a Deep Neural Network (DNN) for handwritten digit recognition using the MNIST dataset.

## Data Preparation
The MNIST dataset is loaded from TensorFlow's datasets, and the data is preprocessed, including:

Scaling the image pixel values by dividing them by 255.
Splitting the data into train, validation, and test sets.
Shuffling the training data using a buffer size of 10,000.

## Model Architecture
The DNN model architecture consists of the following layers:

An input layer that flattens the 28x28 images.
Five hidden layers, with a hidden layer size of 200, and activation functions ReLU and Tanh.
An output layer with 10 units and a softmax activation function for multi-class classification.

## Model Building
The model is created using TensorFlow's Keras API, with the layers defined sequentially. The model is compiled using the Adam optimizer with a learning rate of 0.001, sparse categorical crossentropy loss, and accuracy metric.

## Training and Evaluation
The model is trained on the preprocessed data using the fit() method with a batch size of 100 and for 5 epochs. The time taken for training is also calculated. The model is then evaluated on the test dataset to measure its performance.

## Results
After training, the following results are obtained:

Validation accuracy: 0.9850
Test loss: 0.09
Test accuracy: 97.58%

## Usage
To use this code, simply run the provided Python script. Ensure that you have the required libraries installed, including TensorFlow, NumPy, and TensorFlow Datasets.

## Conclusion
This implementation demonstrates the effectiveness of DNNs in recognizing handwritten digits using the MNIST dataset. The model achieves high accuracy on both training and validation sets.
