# MusAIc – Emotion-Based Music System  

## Introduction  
**MusAIc** is a desktop application designed to enhance the music listening experience by automatically curating playlists based on the user’s current mood. By leveraging facial expression analysis with machine learning, MusAIc simplifies playlist management, allowing users to enjoy music that aligns perfectly with their emotions.  

## Features  
- User authentication using Firebase.  
- Facial expression analysis through webcam image capture.  
- Detection of four primary emotions:  
  - Happy  
  - Sad  
  - Stressed  
  - Surprised  
- Automatic playlist generation based on detected mood.  
- Simple and intuitive user interface for seamless interaction.  

## How It Works  
1. **User Login**:  
   Users log in via Firebase to access their preferences and saved playlists.  
2. **Webcam Access**:  
   The application requests permission to use the webcam to capture the user’s image.  
3. **Emotion Detection**:  
   The captured image is processed using a machine learning model trained on the FER2013 dataset to identify the user’s current emotion.  
4. **Playlist Generation**:  
   Based on the detected emotion, a matching playlist is retrieved from the database and displayed in the application.  
5. **Music Playback**:  
   Users can start playing songs from the curated playlist instantly.  

## Technical Architecture  
- **Frontend**: Built using Flutter and Dart for a responsive and user-friendly interface.  
- **Backend**:  
  - Image processing and facial expression analysis using Python with OpenCV.  
  - Emotion detection powered by a Keras-based Sequential neural network.  
- **Database**: Firebase for user authentication and storing emotion-tagged playlists.  

## System Requirements  
- Python 3.8 or higher.  
- Flutter SDK.  
- Webcam for emotion detection.  
- Required Python libraries:  
  - `opencv-python`  
  - `tensorflow`  
  - `firebase-admin`  

## Installation  
1. Clone the repository:  
   ```bash  
   git clone <repository-link>  
   cd MusAIc  

A few resources to get you started if this is your first Flutter project:

- [Lab: Write your first Flutter app](https://docs.flutter.dev/get-started/codelab)
- [Cookbook: Useful Flutter samples](https://docs.flutter.dev/cookbook)

For help getting started with Flutter development, view the
[online documentation](https://docs.flutter.dev/), which offers tutorials,
samples, guidance on mobile development, and a full API reference.
