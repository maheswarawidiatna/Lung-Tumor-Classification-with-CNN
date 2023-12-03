# Lung Tumor Classification with CNN
[![TensorFlow](https://img.shields.io/badge/TensorFlow-2.0+-orange.svg)](https://www.tensorflow.org/)
[![Bahasa Indonesia](https://img.shields.io/badge/Bahasa-Indonesia-blue.svg)](README.id.md)

## Overview

This script implements a Lung Tumor Classification model using Convolutional Neural Networks (CNN) with the Inception V3 architecture. The model is trained on chest CT scan images to classify tumors into different categories.

## Dependencies

Ensure you have the necessary libraries installed before running the script. You can install them using the following:

```bash
pip install tensorflow pandas matplotlib
```

## Dataset

The dataset used for training and testing is available on Kaggle: [Chest CT Scan Images](https://www.kaggle.com/datasets/mohamedhanyyy/chest-ctscan-images).

To use the Kaggle dataset in the script, upload the `kaggle.json` file, which contains your Kaggle API credentials.

## Script Structure

### 1. Import Libraries

- TensorFlow: For building and training neural networks.
- pandas: For data manipulation and analysis.
- matplotlib.pyplot: For data visualization.

### 2. Upload Dataset via Kaggle API

- Use the Kaggle API to download the chest CT scan dataset.

### 3. Extract ZIP

- Extract the downloaded ZIP file containing the dataset.

### 4. Create Model with Keras and Inception V3

- Load the Inception V3 model with pre-trained weights.
- Modify the model architecture for the tumor classification task.
- Compile the model with categorical crossentropy loss and Adam optimizer.

### 5. Data Augmentation

- Use ImageDataGenerator to perform data augmentation on the training set.

### 6. Learning Phase Model (Epoch 50)

- Train the model on the augmented training set for 50 epochs.
- Monitor and plot the training and validation loss and accuracy.

### 7. Save Model

- Save the trained model for later use.

### 8. Test Predictions with Model on Data Test

- Perform predictions on the test set.
- Convert prediction data to a numpy array.

### 9. Display Predictions

- Display predictions for sample test images along with the predicted class.

Result:

![adafffs](https://github.com/maheswarawidiatna/Lung-Tumor-Classification-with-CNN/assets/94330691/09c40afe-d3f2-41b2-ac32-fc3c7f70a8cb)

**Note:**
- Ensure you have the Kaggle dataset and `kaggle.json` uploaded before running the script.
- Some explanation in the script is written in Bahasa Indonesia
- Feel free to modify the script for your specific use case or dataset.  
