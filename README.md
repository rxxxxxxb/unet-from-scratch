# U-Net from Scratch

This repository contains a from-scratch implementation of the U-Net architecture, a powerful convolutional neural network for biomedical image segmentation. The goal of this project is to provide a clear and easy-to-understand implementation suitable for educational purposes.


## U-Net Architecture

The U-Net architecture is a fully convolutional network that is particularly suited for image segmentation tasks. It consists of two main paths:

- **Encoder (Downsampling Path):** This path captures the context of the input image. It is composed of a series of convolutional and max pooling layers.
- **Decoder (Upsampling Path):** This path enables precise localization. It uses transposed convolutions to upsample the feature maps, which are then concatenated with the corresponding feature maps from the encoder path.

This symmetric, U-shaped architecture enables the network to integrate high-level contextual information with spatial details, resulting in accurate segmentation maps.



## Project Structure

```
. 
├── data
│   ├── images
│   └── annotations
├── notebooks
│   └── training_notebook.ipynb
├── src
│   ├── model.py
│   └── utils.py
├── main.py
└── README.md
```

- **`data/`**: This directory will store the training images and masks.
- **`notebooks/`**: Contains a Jupyter Notebook (`training_notebook.ipynb`) that provides an interactive walkthrough of the training process.
- **`src/`**: Contains the core source code:
    - **`model.py`**: The U-Net model implementation.
    - **`utils.py`**: Helper functions for data loading and preprocessing.
- **`main.py`**: The main training script.
- **`README.md`**: This file.

## Getting Started

### Prerequisites

- Python 3.8+
- PyTorch
- TorchVision
- Pillow
- Requests
