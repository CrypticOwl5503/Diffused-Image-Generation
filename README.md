# Diffusion Generative Model with U-Net Architecture

This repository contains a PyTorch implementation of a diffusion generative model with a U-Net architecture for image generation. The diffusion model is based on the principles of denoising score matching and is trained to generate realistic images from noisy inputs.

## Prerequisites

Before running the code, make sure you have the following dependencies installed:

- Python 3.x
- PyTorch
- NumPy
- Matplotlib
- torchvision
- datasets

You can install the required packages using:

```bash
pip install torch numpy matplotlib torchvision datasets

## Model Architecture
The diffusion model consists of a U-Net architecture with attention blocks and residual blocks. The architecture is designed to capture complex patterns and generate realistic images.

Diffusion: The main model class that incorporates the U-Net architecture with attention and residual blocks.

DDPMSampler: A sampler class used during training to add noise to input images based on the diffusion process.

UNET: U-Net architecture consisting of encoders, a bottleneck layer, and decoders.

UNET_AttentionBlock: Attention block used in the U-Net architecture.

UNET_ResidualBlock: Residual block used in the U-Net architecture.

UNET_OutputLayer: Output layer of the U-Net, producing the final generated image.

## Training
The training script (train.py) loads the MNIST dataset, preprocesses the data, and trains the diffusion model. Training configurations such as epochs, batch size, and learning rate can be adjusted within the script.

## Generation
The generation script (generate.py) generates samples using the trained diffusion model. Adjust the n_inference_steps parameter to control the level of noise in the generated images.

Feel free to explore and modify the code to fit your specific use case or dataset.
