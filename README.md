Plant Disease Detection Using CNN & Streamlit Deployment
Project Overview
This project focuses on detecting plant diseases using deep learning. A Convolutional Neural Network (CNN) was trained on the PlantVillage dataset, which consists of images of diseased and healthy plant leaves. The trained model was then deployed using Streamlit, allowing users to upload images and receive real-time disease predictions.

Dataset
The PlantVillage dataset contains images in three formats:

Color images
Grayscale images
Segmented images
For this project, we used the color images dataset, which contains multiple plant species categorized into healthy and diseased classes.

Project Workflow
Data Preprocessing & Augmentation

Extracted images from the dataset.
Applied ImageDataGenerator to rescale pixel values and split data into training (80%) and validation (20%) sets.
Model Architecture (CNN)

A Sequential CNN model was built with:
Two convolutional layers (Conv2D) with ReLU activation and max pooling.
A fully connected (Dense) layer for classification.
Softmax activation to output probabilities for different disease classes.
Optimizer: Adam
Loss Function: Categorical Crossentropy
Training & Evaluation

The model was trained for 5 epochs with a batch size of 32.
Achieved high validation accuracy on the dataset.
Visualization of Training Performance

Plotted accuracy and loss curves for train and validation sets.
Prediction System

Implemented an image upload function for real-time predictions.
Used argmax on model predictions to classify plant diseases.
Mapped predicted indices to actual class labels.
Deployment with Streamlit

Created an interactive web application using Streamlit.
Users can upload an image of a leaf, and the model predicts whether it is healthy or diseased.
Deployed the model on Streamlit Cloud for accessibility.
