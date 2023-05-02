# Readme
## Introduction
This script is based on "Activities to do on your own" section of the [ConvolutionalVAE notebook](https://git.arts.ac.uk/rfiebrink/ExploringMachineIntelligence_Spring2023/blob/main/week4/ConvolutionalVAE.ipynb) to train a Convolutional Autoencoder on the Dog Breeds Dataset. The script uses Keras with a TensorFlow backend.

## Dataset
The Dog Breeds Dataset contains images of dogs belonging to 120 different breeds. I used a subset of this dataset, containing only images from 9 different breeds. The images in the dataset are of different sizes, so they will be resized to a fixed size of 64x64 before training. The dataset will be manually split into a training set (80% of the data) and a validation set (20% of the data).

## Autoencoder Architecture
The autoencoder architecture consists of an encoder and a decoder. The encoder contains a series of convolutional and pooling layers that reduce the dimensionality of the input. The decoder uses upsampling and deconvolutional layers to reconstruct the original input from the reduced representation.

## Usage
To run the script, make sure you have the following dependencies installed:

- Keras
- TensorFlow
- NumPy
- matplotlib
- argparse
- os
- cv2
To train the autoencoder, run the following command:

You can specify the number of epochs and the batch size as command line arguments. The default values are 50 epochs and 16 batch size.

## Results
The script will output a plot showing the loss and validation loss of the autoencoder during training. It will also display a sample image from the validation set along with its reconstructed image. The autoencoder will be saved as a Keras model file in the current directory.
