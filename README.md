# Smart Fitness Assistant

## Overview
The **Smart Fitness Assistant** is designed to enhance workout experiences by providing real-time feedback and performance tracking. The project flow consists of some features described as follows :

## Key Features
- **Exercise Detection:** The assistant identifies the current workout being performed by the user.
- **Body Orientation Detection:** It then assesses the user's body orientation to ensure proper form and alignment.
- **Repetition Counting:** The system counts the number of repetitions completed for each exercise.
- **Feedback Generation:** Finally, it delivers feedback to the user based on their performance, helping to improve technique and efficiency.
This comprehensive approach aims to support users in achieving their fitness goals while maintaining proper form and reducing the risk of injury.

## Features Descriptions
This section is to explain how each feature works to provide real-time feedback and assistance during your workouts.

### Exercise Detection

The workout detection system is built through a structured process of data collection, processing, and model training, resulting in high-accuracy predictions. Here’s an overview of how this feature works:

1. **Data Collection**: We began by collecting videos for four workout classes (biceps, squats, pushups, and a neutral state) and we have collected data as follows:
   
| Exercise           | Precision           | Recall              | F1-Score          |
|--------------------|---------------------|---------------------|-------------------|
| Squats             | 0.98                | 0.97                | 0.97              |
| Bicep-Curls        | 0.99                | 0.98                | 0.98              |
| Neutral            | 1.00                | 1.00                | 1.00              |
| Push-Ups           | 0.97                | 0.96                | 0.97              |



3. **Keypoint Extraction**: Using the Mediapipe library, we extracted keypoints from the collected videos.

4. **Data Preparation**: The extracted keypoints were saved into a CSV file, which was then split into training and validation sets using an 80:20 ratio.

5. **Data Scaling**: To ensure consistency and improve the performance of the machine learning model, the keypoint data was scaled using a Standard Scaler.

6. **Model Training**: We employed a Random Forest model, which is known for its robustness and accuracy. The model was trained on the scaled keypoint data, achieving an impressive accuracy of 99.26%.

7. **Result**: With this trained model, the system can accurately detect the workout being performed by the user in real time.

| Classification Report | Confusion Matrix |
|-------------------------------|------------------------------|
| ![Keypoint Extraction](path/to/image1.png) | ![Model Accuracy](path/to/image2.png) |
