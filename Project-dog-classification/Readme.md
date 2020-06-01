# Project dog classification

## Project Overview

In this project convolutional neural network is used to predict the dog breed from a given image. If the image has a human instead of a dog the resembling dog breed is predicted. If the image does not have a dog or a human, the app prints the image has neither human nor a dog. The final result is predicted using ResNet50, VGG16 and CV2 Haarcascade architectures.

## Problem statement

The project gets an input of a picture and identifies whether the picture contains a dog or a human. If a dog is detected it predicts the canine’s breed. If a human is detected the project predicts the resembling dog breed. If the application identifies that the image does not have a dog or a human, it prints out the image has neither human nor dog.

## Datasets and inputs

In this project the dataset of 133 different breeds of dogs are being used. A total of 13233 human images and 8351 dog images are used to train, validate and test the model. These images are supplied by Udacity. The model should predict the dog faces with a test set accuracy of 60%

## Benchmark model

Two models are used to compare the predicted dog breeds.

In Model 1 a convolutional neural network is built from scratch to classify dog breeds. This model has three convolutional layers and two fully connected layers to predict the result. The Model is built from scratch and the model predicts a very low accuracy of 13% on test set

In Model 2 a Pytorch pretrained ResNet-50 model is used. Since a pretrained model with 50 layers is used the model has a test set accuracy of 86%.


## Steps involved

The following steps are involved in the final prediction

1. Import Datasets
1. Detect Humans [**(using CV2 Haarcascade)**](https://docs.opencv.org/trunk/db/d28/tutorial_cascade_classifier.html)
1. Detect Dogs [**(using VGG16)**](https://arxiv.org/abs/1409.1556)
1. Create a CNN to Classify Dog Breeds (from Scratch)
1. Create a CNN to Classify Dog Breeds [**(using ResNet-50)**](https://arxiv.org/abs/1512.03385)
1. Write your Algorithm (Implementation)
1. Test Your Algorithm

## Loss function and Optimizer

1. CrossEntropyLoss
2. SGD Optimizer

## Sample Output

The image below displays an potential output if **a dog** is detected on the image.

![Sample output](Images/sample_dog_output.png)

The below image is a potential output if **a human** is detected on the image.

![Sample output](Images/sample_human_output.png)
