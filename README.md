# LW3-Custom-Image-Classifier
## Google Collab Link: 
https://colab.research.google.com/drive/1fFXIVqM-WstrMscIJ11hH5FTaK91AlOq?usp=sharing

# Guide Questions – Answers (Part 1)
# 1. Dataset Preparation
## How did you organize your dataset in Google Drive?

The dataset was organized in a main folder called ImageDataset in Google Drive. Inside this folder, separate subfolders were created for each plant species, and each folder contained images of that specific class. The folder names served as the labels for the dataset.

## Why is folder structure important for TensorFlow image loading?

Folder structure is important because TensorFlow automatically uses the folder names as class labels when loading images using image_dataset_from_directory(). This makes it easier to load and classify images without manually labeling them.

# 2. Model Training
## What is the role of convolutional layers in image classification?

Convolutional layers extract important visual features from images such as edges, textures, and shapes. These features help the model recognize patterns and distinguish between different plant species.

## Why do we split data into training and validation sets?

The dataset is split to evaluate the model’s performance on unseen data. The training set is used to train the model, while the validation set helps check accuracy and detect overfitting.

# 3. Performance Analysis
## What accuracy did your model achieve?

The model achieved a high validation accuracy, showing that it was able to correctly classify most of the plant species images.

## How did the number of images affect the model’s performance?

Having more images per class improved the model’s performance because it provided more examples for the model to learn from.

# 4. Critical Thinking
## What challenges did you encounter while using your own dataset?

Some challenges included collecting enough images for each plant species, organizing the dataset properly, and handling images with different lighting conditions and backgrounds.

## How can data augmentation improve your model?

Data augmentation improves the model by creating variations of existing images through techniques like rotation, flipping, and zooming. This helps the model learn better and improves accuracy.

# 5. Application
## Suggest a real-world application for your trained model.

This model can be used in a plant identification system to help users recognize plant species from images.

## How can this system be integrated into a mobile or web application?

The model can be deployed in a mobile or web app using TensorFlow Lite or TensorFlow.js, allowing users to upload or capture images and receive predictions instantly.

# Activity 3A – Guide Questions Answers (Last Part)
# Visualization & Overfitting
## 1. What signs indicated overfitting in your first model?

In the first model, overfitting was noticeable when the training accuracy kept increasing while the validation accuracy stopped improving or became lower. This showed that the model was learning the training data very well but struggled when predicting new images.

## 2. How did data augmentation affect validation accuracy?

Data augmentation helped improve the validation accuracy because it created different variations of the training images. This made the model learn more patterns and improved its ability to recognize new images.

# Model Improvement
## 3. What is the purpose of dropout layers?

Dropout layers help prevent overfitting by randomly turning off some neurons during training. This forces the model to rely on multiple features instead of memorizing specific patterns in the training data.

## 4. Why does data augmentation improve generalization?

Data augmentation improves generalization because it increases the variety of the training data. Techniques like flipping, rotating, and zooming help the model learn to recognize images even when they appear in different conditions.

# Performance Comparison
## 5. Compare accuracy before and after improvements.

Before applying improvements, there was a larger gap between training and validation accuracy, which indicated overfitting. After applying data augmentation and dropout, the validation accuracy improved and the gap between the two became smaller, showing better model performance.

## 6. Which technique contributed most to improvement?

Both techniques helped improve the model, but data augmentation had the biggest impact because it increased the amount of useful training data and helped the model learn more general features.

# Deployment & Application
## 7. Why is saving the model important?

Saving the model is important because it allows the trained model to be reused later without retraining it again. This saves time and allows the model to be used in applications or systems.

## 8. How can this model be deployed in a real-world system?

The model can be deployed in a mobile or web application where users can upload or take a picture of a plant. The system will process the image and predict the plant species using the trained model.

