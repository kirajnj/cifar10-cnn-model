# cifar10-cnn-model
Implementation and training of a neural network-based model, incorporating enhancements to improve accuracy, using the CIFAR-10 color image dataset.

## Dataset
- Source: CIFAR‑10 by Alex Krizhevsky  
- Link: https://www.cs.toronto.edu/~kriz/cifar.html

## About the project
The notebook cifar10-cnn-model(1).ipynb contains a complete pipeline for training a CNN to recognize 10 classes of images:
airplane, automobile, bird, cat, deer, dog, frog, horse, ship, truck

- Loading and normalization of the CIFAR-10 dataset 
- Convolutional architecture: 4× Conv2D + MaxPooling + Dropout + Dense layers
- Data augmentation (using ImageDataGenerator): rotations, shifts, flips, and zooming
- Model training with validation, including accuracy/loss plots
- Performance evaluation: classification report, confusion matrix, and examples of misclassifications
- Analysis of overfitting

### Results
Validation accuracy: ~76% (best result, epoch 19)
Training accuracy: ~72%
Overfitting: none (gap of ~3%)

Best recognized categories: automobile, truck, ship, horse.
Worst recognized categories: bird, cat, dog (often confused with "frog" or with each other).

<img width="2196" height="788" alt="Снимок экрана 2026-11-03 151323" src="https://github.com/user-attachments/assets/ded888c4-75e9-403a-b245-bbe53419e44c" />
