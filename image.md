# Image Colorization Using U-Net and PyTorch

## Overview
This project implements an image colorization model using a U-Net-inspired deep learning architecture built with PyTorch. The model learns to reconstruct color images from grayscale inputs by training on a dataset of RGB images.

## Features

- Image colorization using deep learning
- U-Net-based neural network architecture
- Custom PyTorch dataset loader
- Automatic grayscale-to-color learning
- Data preprocessing with TorchVision transforms
- Training pipeline using PyTorch

## Dataset Preparation

The notebook:

1. Mounts Google Drive.
2. Extracts an image dataset from a ZIP archive.
3. Loads images from the extracted directory.
4. Converts RGB images to grayscale inputs.
5. Uses original RGB images as training targets.

## Project Workflow

### 1. Environment Setup

Required libraries:

- PyTorch
- TorchVision
- Pillow

```bash
pip install torch torchvision pillow
```

### 2. Data Extraction

The dataset is extracted from a ZIP file stored on Google Drive.

### 3. Data Loading

A custom `ColorizationDataset` class:

- Loads RGB images
- Generates grayscale versions
- Applies image transformations
- Returns grayscale/color image pairs

### 4. Model Architecture

The project uses a U-Net-inspired encoder-decoder architecture.

#### Encoder
- Convolution layers
- ReLU activations
- Max pooling

#### Bottleneck
- Deep feature extraction layer

#### Decoder
- Transposed convolutions for upsampling
- Progressive reconstruction of color information

#### Output Layer
- Produces a 3-channel RGB image

### 5. Training

The model is trained to predict color images from grayscale inputs using supervised learning.

Typical components include:

- Loss function
- Optimizer
- DataLoader
- Backpropagation
- Epoch-based training

## Technologies Used

### Programming Language
- Python

### Libraries
- PyTorch
- TorchVision
- Pillow
- NumPy

## Project Structure

```text
.
├── image_final.ipynb
├── archive.zip
├── extracted_images/
└── image colorization.md
```

## Applications

- Restoration of old black-and-white photographs
- Historical image enhancement
- Computer vision research
- Deep learning experimentation

## Future Improvements

- Improve U-Net architecture with skip connections
- Add validation and testing pipelines
- Train on larger datasets
- Use GAN-based colorization models
- Deploy as a web application

## Author

Ahmed Moniem
