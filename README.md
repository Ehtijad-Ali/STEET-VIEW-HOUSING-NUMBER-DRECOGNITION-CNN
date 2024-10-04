# CNN Model on SVHN Dataset

## Abstract
The Street View House Numbers (SVHN) dataset is a real-world image dataset used for digit recognition. This project involves building and evaluating a Convolutional Neural Network (CNN) model using TensorFlow to classify images from this dataset. The model's performance is analyzed using accuracy, loss metrics, and visualizations.

## 1. Introduction
Digit recognition is a significant challenge in computer vision, with numerous real-world applications such as automatic license plate recognition and postal code sorting. The SVHN dataset consists of over 600,000 labeled digits in natural images. This project leverages CNNs for digit classification due to their ability to capture spatial hierarchies of features effectively.

## 2. Environment Setup
### 2.1. Library Installation
This project requires TensorFlow for deep learning and machine learning tasks. Necessary libraries include TensorFlow, NumPy, Matplotlib, Pandas, and Scikit-learn.

### 2.2. Importing Libraries
Key libraries for data manipulation, visualization, and model building include TensorFlow, NumPy, Matplotlib, and Scikit-learn.

## 3. Data Loading and Preprocessing
### 3.1. Loading the Dataset
The SVHN dataset is loaded using MATLAB file readers, designed to handle the format in which the dataset is stored.

### 3.2. Data Structure
We examine the structure of the dataset to understand how the images and labels are organized.

### 3.3. Data Preparation
The images and labels are reshaped and formatted for TensorFlow. The labels are one-hot encoded for classification purposes.

### 3.4. Data Visualization
We visualize some sample images and their corresponding labels to verify the data quality.

### 3.5. Data Normalization
Pixel values are normalized to a range of [0, 1], and RGB images are converted to grayscale to reduce complexity.

### 3.6. Label Binarization
Labels are converted into one-hot encoded vectors for multiclass classification.

## 4. Model Architecture
### 4.1. Defining the Model
A Convolutional Neural Network (CNN) is defined using the sequential API in TensorFlow. The architecture consists of convolutional layers, pooling layers, batch normalization, and dropout layers.

### 4.2. Model Summary
A summary of the model, including the number of layers and trainable parameters, provides insight into its complexity.

### 4.3. Compiling the Model
The model is compiled with categorical crossentropy loss, the Adam optimizer, and accuracy as the evaluation metric.

## 5. Model Training
### 5.1. Fitting the Model
The model is trained on the training dataset while being validated on the test dataset for several epochs to achieve optimal performance.

### 5.2. Loss and Accuracy Visualization
Loss and accuracy metrics for both training and validation sets are visualized over the course of the training process.

## 6. Model Evaluation
### 6.1. Predictions and Metrics Calculation
Predictions are made on the test set, and performance metrics such as precision, recall, and F1-score are calculated to evaluate the model's performance.

### 6.2. Confusion Matrix and Classification Report
A confusion matrix is generated, and a classification report provides precision, recall, and F1-score for each class, offering a comprehensive view of the model's effectiveness.

### 6.3. Plotting Top 10 Predictions
We visualize the top 10 predictions made by the model, comparing the true and predicted labels along with prediction confidence.

### 6.4. Separate Plots for Test Accuracy Metrics
Separate plots are created to compare test accuracy and maximum validation accuracy during training.

### 6.5. Test Loss
The final test loss is computed to assess the model's generalization performance on unseen data.

## 7. Conclusion
This project demonstrates the successful implementation of a CNN model for digit classification using the SVHN dataset. The model achieves satisfactory accuracy and provides a solid framework for further improvements.

### 7.1. Future Work
Future improvements could include exploring data augmentation techniques to improve model robustness, tuning hyperparameters for optimal performance, and experimenting with more advanced architectures like ResNet or EfficientNet.

## 8. References
#### TensorFlow Documentation
#### SVHN Dataset on Kaggle : https://www.kaggle.com/code/ehtyalee1919/street-view-housing-number-recognition/edit
#### Relevant literature on CNNs and image classification.
