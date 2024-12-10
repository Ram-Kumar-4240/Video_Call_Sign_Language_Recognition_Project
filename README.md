# Video Call Sign Language Recognition Project

## Overview

This project aims to bridge communication gaps for individuals with hearing and speech impairments by integrating real-time sign language recognition into video call applications. It leverages cutting-edge deep learning and computer vision techniques to detect, process, and classify sign language gestures, converting them into text for seamless communication.

## Features
- Sign Language Recognition: Processes video inputs to detect and extract keypoints for sign language gestures using MediaPipe Holistic.
- Keypoint Extraction: Efficient extraction of pose, face, and hand landmarks to represent gestures numerically.
- Data Collection Pipeline: Custom pipeline for capturing and storing video seSequence Modeling: Uses LSTM-based deep learning models to recognize sequences of gestures from video frames.
- Real-Time Text Conversion: Converts recognized gestures into readable text, enabling smooth communication.
- Data Processing Pipeline: End-to-end handling of raw video files, from preprocessing to keypoint extraction and model training.

## Workflow

- Video Data Collection: Processes a dataset of videos annotated with sign language labels.
- Keypoint Extraction: MediaPipe is used to extract pose, face, and hand landmarks, saved as compressed .npz files.
- Data Preprocessing: Sequences of keypoints are padded and normalized for input into the model.
- Model Training:
  - Utilizes LSTM layers for temporal sequence modeling.
  - Supports multi-class classification with categorical encoding of labels.
- Real-Time Inference: Integrates the trained model into a video call system for live gesture-to-text translation.

## Dataset Handling
- Metadata: Processes JSON metadata for video annotation.
- Data Splitting: Divides videos into training, validation, and test sets.
- Error Handling: Skips missing or corrupt files, ensuring robust pipeline execution.

## Technology Stack
- MediaPipe Holistic: Keypoint detection for pose, face, and hand landmarks.
- OpenCV: Video processing and frame extraction.
- TensorFlow/Keras: LSTM-based deep learning model for gesture recognition.
- NumPy: Efficient handling of numerical data and sequences.

## Key Metrics
- Classification Accuracy: Measures the model's ability to predict gestures correctly.
- Real-Time Performance: Ensures minimal latency during live video processing.

## Future Scope
- Expanding the dataset to cover a broader range of gestures and languages.
- Integrating the system with popular video call platforms.
- Enhancing recognition accuracy and real-time performance using advanced architectures like Transformers.

## Usage

Open the Jupyter Notebook to run all stages of the project, including data collection, model training, and real-time prediction. Each section in the notebook is clearly labeled for easy navigation.

## Contributors
- Name : Ramkumar
- Email : infogramrk@gmail.com

