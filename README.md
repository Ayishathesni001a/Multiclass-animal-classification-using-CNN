# Multiclass-animal-classification-using-CNN
# Multi-Class Animal Classification using CNN

A TensorFlow/Keras deep learning project that classifies **15 different animal species** from images using a **Custom Convolutional Neural Network (CNN)**.

![Accuracy Plot](results/accuracy_loss_plot.png)
![Sample Predictions](results/sample_predictions.png)

## 📋 Project Overview

This project builds a multi-class image classifier to identify 15 animal categories. The model is trained from scratch using a custom CNN architecture with data augmentation and regularization techniques.

### Dataset
- **Total Images**: 1,944
- **Training Images**: 1,556
- **Validation Images**: 388
- **Classes**: 15  
  `Bear, Bird, Cat, Cow, Deer, Dog, Dolphin, Elephant, Giraffe, Horse, Kangaroo, Lion, Panda, Tiger, Zebra`

### Model Architecture
- Custom CNN with **5 Convolutional Blocks**
- Batch Normalization after every Conv layer
- Dropout (0.5) in the dense layer
- Input Size: 224 × 224 × 3

### Techniques Used
- Strong Data Augmentation (Flip, Rotation, Zoom, Contrast, Brightness, Translation)
- Early Stopping
- Reduce Learning Rate on Plateau
- Adam Optimizer
- Sparse Categorical Crossentropy Loss

## 📊 Results

| Metric                  | Value     |
|------------------------|-----------|
| Training Accuracy      | **85.93%** |
| Validation Accuracy    | **74.74%** |

The model performs well on distinct animals (Zebra, Elephant, Lion, Dolphin, Cow) but shows confusion between visually similar classes such as Deer ↔ Giraffe and Bird ↔ Cat.

## 📈 Visualizations

### 1. Training History
- Accuracy and Loss curves for both training and validation sets

### 2. Sample Predictions
- 3x3 grid showing actual vs predicted labels with color coding (Green = Correct, Red = Wrong)

## 🚀 How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/animal-classification-cnn.git
   cd animal-classification-cnn
