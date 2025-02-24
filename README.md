# Image Colorization using CNN

## Overview
This project implements a deep learning model for image colorization using a Convolutional Neural Network (CNN) in Keras. The model is trained to take grayscale images as input and predict the `ab` color channels in the Lab color space.

## Project Structure
```
|-- main.py                  # Main script to train and evaluate the model
|-- data_processing.py       # Handles image preprocessing and dataset preparation
|-- model.py                 # Defines the CNN model architecture
|-- train.py                 # Training script
|-- test.py                  # Testing script
|-- requirements.txt         # Dependencies
|-- README.md                # Project documentation
```

## Dependencies
Ensure you have the following libraries installed:
```
numpy
opencv-python
tensorflow
keras
matplotlib
sklearn
```
Install dependencies using:
```
pip install -r requirements.txt
```

## Dataset Preparation
1. Store your grayscale images in a folder (e.g., `dataset/images/`).
2. Update the `ImagePath` variable in the script to point to your dataset directory.
3. The script will process images and convert them into the Lab color space.

## Model Architecture
The model follows an encoder-decoder architecture with convolutional layers:
- Encoder: Extracts features from grayscale images.
- Decoder: Reconstructs the color channels.


