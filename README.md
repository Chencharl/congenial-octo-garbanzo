# congenial-octo-garbanzo
## 🚀Project Overview
This project is a competition from Kaggle, we used a Custom ResNet model for classifying images from the CIFAR-10 dataset. 
The model is trained using PyTorch, incorporating data augmentation, label smoothing, and learning rate scheduling for optimal performance. 
The goal is to maximize test accuracy while keeping the model under 5 million parameters. 

## 📊Dataset
We used the dataset from kaggle: CIFAR-10, which contains 60,000 32x32 color images across 10 classes.

## 🚀Method
We made four versions to continuously optimize the model, and the following are the main methods for our model design:
⚡️RandAugment

⚡️MixUp Implementation

⚡️Rectified Adam

⚡️ReduceLROnPlateau

## Summary of Architectural Changes Across Versions

| Version | Key Changes |
|---------|------------|
| **V1**  | Initial ResNet design with 3 residual blocks. |
| **V2**  | Introduced MixUp data augmentation to improve generalization. |
| **V3**  | Increased depth (added residual blocks), reduced initial channels (64→32), restructured feature extraction. |
| **V4**  | Switched optimizer to RAdam, introduced learning rate scheduler, adjusted training epochs. |


## 🚀Conclusion
Finally, achieved almost 90% accuracy on the CIFAR-10 dataset on local running and successfully kept parameters under 5 million.


## 📃Files
main.ipynb – Contains the final version of the model with the best performance. Run this file to reproduce the results.
model_optimization_versions.ipynb – Shows the model optimization process, including different versions and improvements made.

## 🔗Reference
Zhang, H.; Cisse, M.; Dauphin, Y. N.; and Lopez-Paz, D. 2017. Mixup: Beyond empirical risk minimization. In International Conference on Learning Representations (ICLR).

## ✨Contributors
Yinuo Wang yw8041@nyu.edu
Chen Yang cy2683@nyu.edu
Jiale Cai jc12423@nyu.edu
