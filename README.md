# FaceMask-Detection

## Overview

This repository implements a deep learning-based face mask detection system using **PyTorch** and **MobileNetV2** architecture. The model classifies images into two classes:

- `with_mask`
- `without_mask`

The project includes a complete pipeline for data preprocessing, training, validation, evaluation, and inference.

---

## Features

- MobileNetV2 architecture optimized for face mask detection.
- Data augmentation to improve generalization.
- Automatic train-validation split.
- Training progress visualization including accuracy and loss curves.
- Model saving and loading for inference.
- Sample prediction on test images.

---

## Repository Structure

| File/Folder              | Description                              |
|-------------------------|------------------------------------------|
| `facemask-detection.ipynb` | Jupyter notebook with full training and evaluation code |
| `requirements.txt`       | List of required Python packages          |
| `face_mask.pth`          | Trained model weights                      |
| `Outputs/`               | Folder containing outputs images |

---

## Model Architecture Details

| Parameter                | Value                                  |
|-------------------------|----------------------------------------|
| Base Model              | MobileNetV2                            |
| Input Image Size        | 224 x 224 pixels                      |
| Number of Classes       | 2 (with_mask, without_mask)            |
| Optimizer               | Adam                                 |
| Learning Rate           | 0.001                                |
| Loss Function           | CrossEntropyLoss                     |
| Batch Size              | 32                                   |
| Number of Epochs        | 20                                   |

---

## Installation

```bash
git clone https://github.com/suman2896/FaceMask-Detection.git
cd FaceMask-Detection
pip install -r requirements.txt
