# Emotion-based-music-recommendation

# Emotion-Based Music Recommender

## Overview

This project uses real-time emotion detection to recommend music based on the user's facial expressions and hand gestures. It employs various technologies such as Streamlit, OpenCV, MediaPipe, Keras, and TensorFlow to provide an interactive web-based application.

## Features

- **Real-time Emotion Detection**: Captures video input from the webcam to detect the user's emotions.
- **Personalized Music Recommendations**: Recommends music based on the detected emotion, preferred language, and singer.
- **Web Interface**: Simple and interactive user interface built with Streamlit.

## Technologies Used

- **Streamlit**: For creating the web interface.
- **Streamlit WebRTC**: For real-time video streaming.
- **OpenCV (cv2)**: For image processing.
- **NumPy**: For numerical operations.
- **MediaPipe**: For facial and hand landmarks detection.
- **Keras**: For loading and running the pre-trained emotion detection model.
- **TensorFlow**: Backend for Keras.
- **Webbrowser**: To open URLs in the web browser.

## Setup and Installation

1. **Clone the repository:**
    ```bash
    git clone https://github.com/your-username/emotion-based-music-recommender.git
    cd emotion-based-music-recommender
    ```

2. **Create and activate a virtual environment:**
    ```bash
    python -m venv venv
    source venv/bin/activate   # On Windows: venv\Scripts\activate
    ```

3. **Install the required dependencies:**
    ```bash
    pip install -r requirements.txt
    ```

4. **Download or prepare the model and labels:**
    - Ensure you have the `model.h5` file in the root directory.
    - Ensure you have the `labels.npy` file in the root directory.

## Usage

1. **Run the Streamlit application:**
    ```bash
    streamlit run music.py
    ```

2. **Interact with the web interface:**
    - Enter your preferred language and singer in the provided text input fields.
    - Allow the application to capture video from your webcam to detect your emotion.
    - Once an emotion is detected, click the "Recommend me songs" button to open YouTube with a personalized music recommendation.

## Project Structure

```plaintext
emotion-based-music-recommender/
│
├── model.h5
├── labels.npy
├── music.py
├── requirements.txt
└── README.md
