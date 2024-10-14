# CNN for Lung Disease Detection in X-ray Images

## Overview
This project explores the use of various **Convolutional Neural Network (CNN)** architectures to classify chest X-ray images into three categories: **COVID-19**, **pneumonia**, and **normal**. We developed and compared several CNN models, progressively introducing advanced features like **Depthwise Separable Convolutions**, **Attention Mechanisms**, and **DenseNet architectures**, all while maintaining consistent training settings to ensure fair comparison.

## Models and Architectures
The following CNN architectures were implemented and compared:

1. **Basic CNN**: A standard CNN architecture used as a baseline model.
2. **Depthwise CNN**: Optimized for computational efficiency using Depthwise Separable Convolutions, providing the best trade-off between accuracy and performance.
3. **Attention CNN**: Incorporates spatial attention mechanisms to focus on diagnostically relevant regions of X-ray images.
4. **DenseNet**: Utilizes dense connectivity between layers to promote feature reuse and improve gradient flow.

## Dataset
- The dataset consists of **4575 chest X-ray images** (1525 images per class: COVID-19, pneumonia, and normal).
- Images were resized to **224x224 pixels**, and the dataset was split into **training (80%)**, **validation (10%)**, and **test (10%)** sets.

## Key Techniques
- **Data Augmentation**: Random rotations, zooms, and translations were applied to the training data to prevent overfitting.
- **Feature Extraction**: Each CNN architecture includes progressively more advanced layers for optimized feature extraction.
- **Regularization**: Dropout layers and batch normalization were used to prevent overfitting and stabilize training.

## Results
The **Depthwise CNN** emerged as the most effective model, achieving:
- **Accuracy**: 87.06%
- **Precision**: 96.19%
- **Recall**: 88.39%
- **F1-score**: 92.12%
- **Area Under Curve (AUC)**: High across all classes

Other models, such as the **Attention CNN**, showed promise in reducing misclassification between COVID-19 and normal cases but lagged in overall performance compared to Depthwise CNN.

## Inference Efficiency
We evaluated the models on:
- **Inference Time**: The time taken to process a single image.
- **Memory Usage**: The computational resources required for deployment.
  
The **Basic CNN** showed the fastest inference time but suffered from high memory usage, while the **Depthwise CNN** offered a balanced solution with efficient inference time and minimal memory footprint.

## Conclusion
The **Depthwise CNN** is the most suitable model for real-world deployment in medical diagnostics due to its high classification accuracy and resource efficiency. Further tuning of models like the **Attention CNN** could improve performance in more critical diagnostic tasks.
