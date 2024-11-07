# Automated Tumor Detection in Medical Images

## Overview
This project aims to develop a Convolutional Neural Network (CNN) model for early detection of lung cancer nodules using chest CT scan images. Early and accurate diagnosis of lung tumors is crucial for improving patient outcomes. The model processes CT scan images and classifies them into three categories: Normal, Benign, and Malignant cases.

## Dataset
The dataset used for this project consists of CT scan images sourced from medical imaging datasets, such as Kaggle and IQ-OTHNCCD. These datasets provide annotated data essential for training and validating CNNs.
This Dataset includes a total of 1190 CT scan images.

## Challenges Addressed
* Automation and Efficiency: Leveraging AI to automate the tumor detection process, reducing manual interpretation.
* Accuracy: Using machine learning algorithms to minimize false positives and false negatives, improving the reliability of detection.
* Consistency: Providing consistent and objective results through standardized image interpretation.

## Data Preparation
* Image Preprocessing:
* Load images from respective folders
* Convert to grayscale
* Resize to 256x256 pixels
* Apply Label Mapping:
   Normal cases: 0
   Benign cases: 1
   Malignant cases: 2

## Model Architecture
The model is based on a deep Convolutional Neural Network (CNN) model using Keras, which consists of multiple convolutional, pooling, and dropout layers to enhance learning and prevent overfitting. The final layer uses a softmax activation function to classify the images into the three categories. The model is trained using the Adam optimizer and sparse categorical crossentropy as the loss function.
  
The training process shows a consistent decrease in loss and an increase in accuracy over the epochs.

## Model Performance
* Validation Accuracy: Peaked at 98.30%
* Confusion Matrix: Indicates strong performance across all categories (Normal, Benign, Malignant).

## Results
The model demonstrates high accuracy and effective learning on both training and validation datasets.
The confusion matrix further confirms the model's ability to classify images correctly.

## Future Enhancements 
Several key improvements can be explored to enhance the performance and applicability of the lung cancer detection model. First, hyperparameter tuning should be pursued to optimize parameters such as learning rate, batch size, and the number of layers, which could lead to improved model performance and stability. Additionally, experimenting with advanced model architectures, including deeper networks or transfer learning approaches, may offer better feature extraction and classification accuracy, particularly in complex medical imaging tasks. Incorporating more diverse datasets is another crucial step to improve the model's ability to generalize to a wider variety of cases, making it more robust when handling new or unseen data. Lastly, evaluating the model on real-world clinical data will be essential for assessing its practical applicability in a healthcare setting, ensuring it can reliably detect lung cancer in real diagnostic environments.
