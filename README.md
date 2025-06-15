# 🔥 Wildfire Detection from Images using Deep Learning

This project uses deep learning models to detect wildfires from visual images. Our goal is to build accurate and robust fire detection systems that can work in real-world settings with limited data and ambiguous visual cues.

## Overview

Wildfire detection is crucial for preventing large-scale damage to the environment, human life, and property. In this project, we compare multiple deep learning approaches, including ResNet and Vision Transformers (ViT), to classify images as either `fire` or `no fire`.

Key features:
- Training models from scratch and fine-tuning pretrained ones.
- Handling class imbalance through class-weighted loss functions.
- Synthetic image generation using diffusion models.
- Real-time data augmentation pipeline for small datasets.

## Dataset

We use [The Wildfire Dataset](https://www.kaggle.com/datasets/elmadafri/the-wildfire-dataset), which contains images labeled as `fire` or `no fire`, split into train, validation, and test sets.

We augment and generate new images to improve training with this limited dataset.

## Models Used

- **ResNet-18 (from scratch)**: A basic convolutional neural network trained without any pretraining.
- **ResNet-18 (pretrained)**: Fine-tuned on our wildfire dataset after pretraining on ImageNet.
- **Vision Transformer (ViT-base-patch16-224)**: Captures long-range dependencies in images.

## Installation

Clone this repository:
   ```bash
   git clone https://github.com/yourusername/wildfire-detection.git
   cd wildfire-detection
