# congenial-octo-garbanzo
## Project Overview
This project is a competition from Kaggle, we used a Custom ResNet model for classifying images from the CIFAR-10 dataset. 
The model is trained using PyTorch, incorporating data augmentation, label smoothing, and learning rate scheduling for optimal performance. 
The goal is to maximize test accuracy while keeping the model under 5 million parameters. 

## Dataset
We used the dataset from kaggle: CIFAR-10, which contains 60,000 32x32 color images across 10 classes.
## Project Procedure
### Data Preparation
#### Load the CIFAR-10 Dataset
#### Data Augmentation and Normalization
#### Split the training and validation sets
90% of the images were used for training, while 10% were reserved for validation.
The dataset was converted into PyTorch tensors for efficient batch processing.
