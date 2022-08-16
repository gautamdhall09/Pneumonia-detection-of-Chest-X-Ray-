# CNN to detect Pneumonia using Chest X-Rays

## Overview
A Convolutional Neural Net (CNN/ConvNet) is a Deep Neural Network, that takes inputs as images, assigns weights and biases to various aspects of the image and
then differentiates among different class of images. The pre-processing required in a ConvNet is much lower as compared to other classification algorithms.
A ConvNet is able to successfully capture the Spatial and Temporal dependencies in an image through the application of relevant filters. The architecture performs a better fitting to the image dataset,
when compared to a standard neural network, due to the reduction in the number of parameters involved and reusability of weights.

## About this Project
This repository contains a self-made ConvNet (CNN.py) implemented using Keras, an open source neural network library in Python. The model is
computationally cheaper than other popular and successful implementations of CNNs such as the VGG16 and ResNet50, having only
77,633 trainable parameters compared to the 138,000,000 parameters of VGG16 and 23,000,000 parameters of ResNet50.

Despite it's low number of parameters, it manages a **training set accuracy ~ 96%** and **test set accuracy ~ 93%**.

It uses 7 Convolution and Pooling layers along with Spatial Dropout to prevent overfitting, followed by 3 Dense and Dropout layers to classify the images
as having pneumonia (both viral and bacterial) or not having pneumonia.

## About the Dataset
The dataset used is avaiable on [Kaggle](www.kaggle.com) and consists of 5863 images divided into two classes. For the analysis of chest x-ray images, all chest radiographs were initially screened for quality control by removing all low quality or unreadable scans. The diagnoses for the images were then graded by two expert physicians before being cleared for training the AI system.

You can access the dataset [here](https://www.kaggle.com/paultimothymooney/chest-xray-pneumonia)

![yo](https://i.imgur.com/jZqpV51.png)

This figure illustrates examples of chest X-rays in patients with pneumonia.

The normal chest X-ray (left panel) depicts clear lungs without any areas of abnormal opacification in the image. Bacterial pneumonia (middle) typically exhibits a focal lobar consolidation, in this case in the right upper lobe (white arrows), whereas viral pneumonia (right) manifests with a more diffuse ‘‘interstitial’’ pattern in both lungs

Please note that the model does not differentiate between viral and bacterial pneumonia.








