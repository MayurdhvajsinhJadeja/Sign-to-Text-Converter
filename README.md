# Sign Language to Text Prediction System

A machine learning system that translates sign language gestures into text through hand and palm detection.

## Overview

This system analyzes hand gestures to interpret and convert sign language into text. It uses computer vision and machine learning techniques to detect hand landmarks, calculate relevant distances and transformations, and predict the corresponding text or meaning based on these features.

## Project Pipeline

1. **Data Collection**
   - Creating a dataset of sign language gestures for training and testing

2. **Hand Detection**
   - Using MediaPipe for initial hand detection
   - Palm Detection Model locates the palm in images
   - Hand Landmarks Detection Model identifies key points on the hand

3. **Feature Engineering**
   - Origin Transform: Converting hand coordinates to a normalized reference frame
   - Distance Calculation: Measuring distances between landmarks
   - New Coordinate Distance calculation to extract meaningful features for sign recognition

4. **Model Training**
   - Machine learning model trained on the extracted features
   - Outputs predicted sign language class or text equivalent

5. **Visualization**
   - Results displayed on Python GUI for development purposes

![image](https://github.com/user-attachments/assets/ac0718c8-a1a4-44a8-966c-9c0661fd2048)

## Requirements

- Python 3.x
- MediaPipe
- OpenCV
- TensorFlow/PyTorch (for ML model)
