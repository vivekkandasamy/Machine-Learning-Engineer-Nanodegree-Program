# Project dog classification

## Project Overview

In this project convolutional neural network is used to predict the dog breed from a given image. If the image has a human instead of a dog the resembling dog breed is predicted. If the image does not have a dog or a human, the app prints the image has neither human nor a dog. The final result is predicted using ResNet50, VGG16 and CV2 Haarcascade architectures.

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
