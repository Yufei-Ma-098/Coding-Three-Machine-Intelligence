# Readme
This is the code for a Variational Autoencoder (VAE) that can generate new images of dogs.

## Data
The data used for this project is a collection of images of dogs, stored as a CSV file (dogs.csv) that contains the filepaths to the images. Only a small subset of the images (500) is used to save memory.

## VAE Architecture
The VAE consists of an encoder and a decoder. The encoder takes in an input image and outputs the mean and variance of the latent space distribution. The decoder takes in a sample from the latent space and decodes it into an image.

The architecture of the encoder is as follows:

- Input layer with shape `(64, 64, 1)`
- Two convolutional layers with 32 and 64 filters, respectively, with kernel size 3, stride 2, and 'same' padding, followed by ReLU activation
- Flatten layer
- Dense layer with 16 units, followed by ReLU activation
- Two dense layers that output the mean and log-variance of the latent space distribution, respectively
- The architecture of the decoder is as follows:

Input layer with shape `(latent_dim,)`
- Dense layer with `16 * 16 * 64` units, followed by ReLU activation
- Reshape layer to reshape the output of the dense layer into a 3D tensor with shape `(16, 16, 64)`
- Two transpose convolutional layers with 64 and 32 filters, respectively, with kernel size 3, stride 2, and 'same' padding, followed by ReLU activation
- Output layer with one filter and kernel size 3, followed by sigmoid activation

# Training
The VAE is trained on the dog images using the `vae_loss` function, which is a combination of the reconstruction loss (binary cross-entropy) and the KL divergence loss between the latent space distribution and a standard normal distribution.

The trained encoder and decoder models are saved to disk as `encoder.h5` and `decoder.h5`, respectively.

# Generating Images
The `plot_generated_images` function can be used to generate and plot new images of dogs by sampling from the latent space and decoding the samples using the trained decoder model.

# Requirements
- Python 3
- TensorFlow 2
- NumPy
- pandas
- matplotlib
- OpenCV (cv2)
