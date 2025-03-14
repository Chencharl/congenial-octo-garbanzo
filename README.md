# congenial-octo-garbanzo
## 🚀Project Overview
This project is a competition from Kaggle, we used a Custom ResNet model for classifying images from the CIFAR-10 dataset. 
The model is trained using PyTorch, incorporating data augmentation, label smoothing, and learning rate scheduling for optimal performance. 
The goal is to maximize test accuracy while keeping the model under 5 million parameters. 

## 📊Dataset
We used the dataset from kaggle: CIFAR-10, which contains 60,000 32x32 color images across 10 classes.
## 🚀Project Procedure
### 💡Method
#### ⚡️Load the CIFAR-10 Dataset
#### ⚡️Data Augmentation and Normalization
#### ⚡️Split the training and validation sets
90% of the images were used for training, while 10% were reserved for validation.
The dataset was converted into PyTorch tensors for efficient batch processing.
#### ⚡️Model Design
We made five versions to continuously optimize the model, and the following is our model design for each version。
The First Version，initial design with an initial convolutional layer followed by three residual blocks (ResidualBlock).  
The Second Version, MixUp Data Augmentation, implementing the mixup_data function to linearly mix images and labels during training with α=0.2. 
The Third Version, expanded the model’s depth by adding additional residual blocks to each stage, restructuring each stage to contain three stacked residual blocks instead of two.  
The Fourth Version, focused on optimizing training efficiency and model stability. 
These changes collectively improved the model’s performance and stability during training.
## 🚀Conclusion
Finally, achieved almost 90% accuracy on the CIFAR-10 dataset and successfully kept parameters under 5 million.
## 🔗Reference
Zhang, H.; Cisse, M.; Dauphin, Y. N.; and Lopez-Paz, D. 2017. Mixup: Beyond empirical risk minimization. In International Conference on Learning Representations (ICLR).
## ✨Contributors
Yinuo Wang yw8041@nyu.edu
Chen Yang cy2683@nyu.edu
Jiale Cai jc12423@nyu.edu
