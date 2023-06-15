# Readme
This is a simple implementation of a GAN using TensorFlow 2. The code is based on [dcgan.ipynb](https://git.arts.ac.uk/rfiebrink/ExploringMachineIntelligence_Spring2023/blob/main/week5/dcgan.ipynb), but with a modification to the activation function in the generator model. Specifically, I changed the activation function from LeakyReLU to ReLU, which led to a noticeable improvement in the quality of the generated images.

## Changes Made
The only change made to the original code was to the `make_generator_model function`. I replaced all instances of `tf.keras.layers.LeakyReLU` with `tf.keras.layers.ReLU`. This allowed the generator model to better capture the underlying structure of the dataset, which resulted in higher quality generated images.

## Usage
To run the code, simply run the train function. You can specify the number of epochs to train for and the batch size by changing the `EPOCHS` and `BATCH_SIZE` variables at the beginning of the code.

After training is complete, the `generate_and_save_images` function can be used to `generate and save images` from the trained generator model.

## Dependencies
The code requires the following dependencies:

- TensorFlow 2
- NumPy
- Matplotlib
- imageio

## Acknowledgments
The code is based on the TensorFlow 2 GAN tutorial, which can be found [here](https://www.tensorflow.org/tutorials/generative/dcgan).
