# Smart Fitness Assistant

## Overview
The **Smart Fitness Assistant** is a Python-based application designed to provide real-time feedback and guidance for fitness exercises. Leveraging computer vision and machine learning techniques, this app helps users improve their workout techniques and achieve their fitness goals.

## Features
- **Exercise Detection:** Utilizes a YOLOv8 model to detect keypoints for various exercises (biceps curls, squats, pushups).
- **Real-time Feedback:** Provides instant feedback on user form and technique during workouts.
- **Custom Workouts:** Users can select from different workout routines tailored to their fitness level.
- **Video & Image Output:** Generates videos and images to visualize the workout performance and improvements over time.

## Technologies Used
- Python 3.9
- OpenCV
- Mediapipe
- YOLOv8
- Streamlit for web deployment
- NumPy, Pandas, and other essential libraries

## Getting Started
To set up the project locally, follow these steps:

### Prerequisites
Make sure you have Python 3.9 installed. You can check your version with:
```bash
python --version
