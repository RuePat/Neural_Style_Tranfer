# Neural_Style_Tranfer

Neural Style Transfer using VGG19
This repository contains a Python implementation of Neural Style Transfer using the VGG19 model. Neural Style Transfer is a technique to generate an image that combines the content of one image with the style of another image. The VGG19 model is utilized as a feature extractor to separate and capture content and style information from images.

Installation
Make sure you have Python installed along with pip. You can install the required dependencies using the following command:

!pip install torch torchvision matplotlib

Usage
Load VGG Pretrained Model:

The VGG19 model pretrained on ImageNet is loaded using PyTorch.

Preprocess Image:

Images are preprocessed to fit the model input requirements. Resize the image to the desired size and apply normalization.

Deprocess Image:

Deprocessing involves reverting the processed image back to its original form by undoing the normalization.

Get Features:

Extract features from the images using the VGG19 model. Features are extracted at specific layers to capture content and style information.

Gram Matrix Calculation:

Calculate the Gram matrix from the feature maps to represent the style of an image.

Loss Functions:

Define content loss and style loss functions to quantify the difference between the generated image and the content image, and the difference between the style of the generated image and the style image, respectively.

Training Loop:

Utilize an optimization algorithm (Adam optimizer) to minimize the total loss, which is a combination of content loss and style loss. Adjust the weights (alpha and beta) to control the contribution of each loss.

Example
An example of Neural Style Transfer is demonstrated by combining the content of one image with the style of another image.
