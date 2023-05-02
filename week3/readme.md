# Readme
This code is used to classify the Fashion MNIST dataset using CNN implemented with TensorFlow and Keras.

## Dataset
The Fashion MNIST dataset is used for this classification task, which contains 60,000 28x28 grayscale images of 10 fashion categories, and 10,000 test images. The dataset is included in Keras.

## Preprocessing
The dataset is preprocessed by reshaping the images to 28x28x1, converting the pixel values to float32 and normalizing them between 0 and 1. The labels are converted to one-hot encoding.

## Model Architecture
The model architecture consists of a series of convolutional layers, max pooling layers, a flattening layer, and fully connected layers. The final output layer uses softmax activation to output the classification probabilities.

## Training
The model is trained for 10 epochs with a batch size of 32. The loss function used is categorical cross-entropy and the optimizer used is Adam. The model is also evaluated on the test set.

