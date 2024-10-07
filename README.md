# Umpire-Sign-Recognition

## Objective
The primary objective of this project is to develop a Convolutional Neural Network (CNN) model capable of recognizing different hand signs from a live webcam feed. This model can be utilized for various applications, including gesture-based control systems and sign language interpretation.

## Problem Statement
Umpire sign recognition is a crucial component in developing human-computer interaction systems, especially for individuals cricket fans with speech or hearing impairments. The challenge lies in accurately detecting and classifying cricket signs from real-time video input, where variations in lighting, background, and hand positioning can affect the model's performance.

## Dataset
The dataset for this project is generated using the `Create.ipynb` notebook, which captures images from a webcam. The images are pre-processed, including hand segmentation from the background, and saved for training the model. The dataset includes multiple hand sign classes, each represented by a set of images.

## Working of the Project
1. **Dataset Creation**: 
   - The `Create.ipynb` notebook is used to capture images from a webcam. The Region of Interest (ROI) is defined, and each frame is processed to segment the hand from the background. The segmented images are saved for training.
   
2. **Model Training**:
   - A CNN model is trained using the generated dataset. The model learns to recognize different hand signs by learning the unique features of each sign.
   
3. **Real-time Prediction**:
   - The `Predict.ipynb` notebook loads the trained model and uses it to predict hand signs in real-time. The live video feed is captured from a webcam, and each frame is processed to segment the hand. The segmented image is then fed to the model, which predicts the hand sign.

## What is Included in Each Python File

### 1. `Create.ipynb`
  - Captures and initializes the background for subsequent hand segmentation.
  - Segments the hand from the background in each frame.
  - Saves the segmented hand images into the specified directory for each hand sign class.

### 2. `Predict.ipynb`
  - Loads the pre-trained hand sign recognition model.
  - Segments the hand from the background in real-time.
  - Predicts the hand sign shown within the Region of Interest (ROI) using the CNN model.

## Conclusion
This project demonstrates the application of CNNs in real-time umpire sign recognition. The system developed can be further expanded to recognize a broader set of gestures.

