# Subverting the Chairs: StyleGAN XL with Random Prompt Outputs
This is a project that generates random chair images using the StyleGAN XL and OpenAI's CLIP model for guidance based on text inputs. The unique feature of this code is the ability to generate random prompts, which includes varying combinations of colors, styles and events.

The code relies on CLIP's text-to-image capabilities to guide the StyleGAN model, generating images that align with a given text prompt. This project stands out with its capacity to generate random prompts, providing unique text inputs to guide the image generation process.

## Project Theme
Chairs serve as an embodiment of public flux and disorder. They stand as a medium, establishing the connection between humans and the infinite. As we sit in chairs to work, ponder, converse, and even sleep, these stationary objects bear witness to our fluid nature.

Utilizing StyleGAN technology, I've curated an array of chairs in various styles, strange and wonderful. They cease to be singular or static. This is a challenge to conventional perceptions of chairs, but moreover, it's an opportunity to rethink our human culture.

## Installation and Running the Code
This project is designed to run in Google Colab.

## Technical Details
The code begins by installing necessary libraries and cloning repositories for StyleGAN XL, CLIP and ESGD and sets the device to CUDA if available.

Then the code generates random text prompts by selecting a random choice of colors, styles and events. These prompts guide the model to generate images.

The images are generated in a sequence and displayed in the notebook. Once the image generation process is complete, these images are saved into a video file, providing a transition between the different image outputs.

## Libraries and Models Used:
- **StyleGAN XL:** This is an enhanced version of the original StyleGAN model, optimized for generating high-resolution images.
- **CLIP (Contrastive Language–Image Pretraining):** This model from OpenAI uses transformers to connect images and text, providing a way to guide the image generation process.
ESGD (Evolution Strategies with Stochastic Gradients): This library provides the optimization algorithm used in the training process.

## Important Functions:
- **fetch:** This function fetches an image from a URL or a file path.
- **fetch_model:** This function fetches a StyleGAN model from a URL.
- **slugify:** This function converts a given string to a format that can be used in a URL or filename.
- **spherical_dist_loss:** This function calculates the spherical distance loss.
- **prompts_dist_loss:** This function calculates the prompt distance loss.
- **run:** This function runs the entire image generation process.

## Reference Code and Libraries
- [StyleganXL](https://github.com/autonomousvision/stylegan-xl)
- [CLIP](https://github.com/openai/CLIP)
- [StyleGAN3-CLIP](https://github.com/ouhenio/StyleGAN3-CLIP-notebooks)
- [gen-clip](https://github.com/ryudrigo/my-gen-clip)
