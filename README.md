# U-Net from Scratch

This repository contains a from-scratch implementation of the U-Net architecture, a powerful convolutional neural network for biomedical image segmentation. The goal of this project is to provide a clear and easy-to-understand implementation suitable for educational purposes.


## U-Net Architecture

The U-Net architecture is a fully convolutional network that is particularly suited for image segmentation tasks. It consists of two main paths:

- **Encoder (Downsampling Path):** This path captures the context of the input image. It is composed of a series of convolutional and max pooling layers.
- **Decoder (Upsampling Path):** This path enables precise localization. It uses transposed convolutions to upsample the feature maps, which are then concatenated with the corresponding feature maps from the encoder path.

This symmetric, U-shaped architecture enables the network to integrate high-level contextual information with spatial details, resulting in accurate segmentation maps.
