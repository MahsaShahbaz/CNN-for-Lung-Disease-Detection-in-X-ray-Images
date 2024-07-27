# CNN-for-Lung-Disease-Detection-in-X-ray-Images
Lung Disease Detection in X-ray Images using CNNs

This project explores the use of convolutional neural networks (CNNs) to classify X-ray images into three categories: COVID-19, pneumonia, and normal. It includes data preprocessing, augmentation, and model development using various CNN architectures. The models evaluated include a basic CNN, depthwise CNN, CNN with attention mechanisms, and DenseNet.


Introduction:

The COVID-19 pandemic has highlighted the need for rapid and accurate diagnostic tools. This project aims to develop and evaluate CNN architectures for classifying chest X-ray images, which can assist in diagnosing COVID-19, pneumonia, and distinguishing them from normal cases.


Dataset:

The dataset used consists of chest X-ray images categorized into three classes: COVID-19, pneumonia, and normal. The dataset is split into training, validation, and test sets. The directory structure is as follows:


COVID19

Normal

Pneumonia

The dataset contains a total of 4575 images, equally distributed among the three classes.


Data Preprocessing:

Data preprocessing includes normalization and data augmentation:

Normalization: 
Scaling pixel values to the range [0, 1].

Augmentation: 
Techniques such as random rotation, zoom, and translation are applied to the training dataset to increase robustness and prevent overfitting.


Model Architectures:

We experimented with multiple CNN architectures:


Basic CNN: 

A straightforward CNN with several convolutional and max-pooling layers.

Depthwise CNN: 

An advanced CNN that includes depthwise separable convolutions for efficient feature extraction.

Attention CNN: 

A CNN that incorporates attention mechanisms to focus on the most relevant parts of the images.

DenseNet: 

A densely connected convolutional network using dense blocks and transition layers.


Training and Evaluation: 

The models are trained on the training dataset and validated on the validation dataset. Various metrics are used to monitor performance, including accuracy, loss, precision, recall, AUC, and F1 score.

Results: 
The Basic CNN outperformed other architectures with a training accuracy of 99.01%, precision of 95.20%, recall of 90.41%, and F1-score of 89.79%. The depthwise CNN, attention CNN, and DenseNet achieved training accuracies of 91.95%, 83.03%, and 85.96%, respectively.

Contributing: 
Contributions are welcome! Please fork the repository and submit pull requests.
