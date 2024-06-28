# Brain Tumor Segmentation using Lightweight U-Net

## Overview
This project focuses on the segmentation of brain tumors from MRI scans using a lightweight implementation of the U-Net architecture. The model is designed to provide real-time segmentation without the need for large amounts of training data or additional data augmentation steps. The lightweight U-Net demonstrates promising results on the transversal plane , achieving a mean intersection-over-union (IoU) of 90% and outperforming standard benchmark algorithms.

## Table of Contents
- [Introduction](#introduction)
- [Dataset](#dataset)
- [Model Architecture](#model-architecture)
- [Training](#training)
- [Evaluation](#evaluation)
- [Results](#results)
- [Installation](#installation)
- [Usage](#usage)
- [References](#references)

## Introduction
Brain tumor segmentation in MRI scans is a critical task in medical imaging, enabling precise treatment planning and diagnosis. This project implements a lightweight U-Net model to segment tumors in brain MRI scans efficiently.

## Dataset
The BITE dataset is used for training and evaluation. It consists of MRI scans with corresponding tumor masks. In this project, already sliced images are used, simplifying the preprocessing steps and allowing for more focused segmentation tasks.

## Model Architecture
The model is based on the U-Net architecture with several modifications to reduce its complexity and computational requirements. The architecture comprises:
- Convolutional layers with filters of sizes 64, 128, and 256.
- Batch normalization and ReLU activations.
- Max pooling for downsampling.
- UpSampling and concatenation for upsampling.

## Training
The model is trained using the Adam optimizer with a learning rate of 1e-4 and a batch size of 8. Key metrics used during training include pixel accuracy, mean accuracy, mean IoU, and frequency-weighted IoU. Early stopping, model checkpointing, and learning rate reduction are applied to enhance training efficiency.

## Evaluation
The model is evaluated on a test set to measure its performance using the aforementioned metrics. The evaluation script generates quantitative metrics and visualizes the segmentation results.

## Results
The lightweight U-Net achieves a mean IoU of 90% on the BITE dataset, demonstrating its effectiveness in brain tumor segmentation. where results are saved in evaluation.txt file
## Installation
To set up the project, follow these steps:

1. Clone the repository:
   ```bash
   https://github.com/hiranmayee13/brain-tumor.git

