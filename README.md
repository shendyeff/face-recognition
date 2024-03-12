# **Documentation Face Recognition System with OpenCV**

## Project Description
This project aims to develop a face recognition system using LBPH (Local Binary Patterns Histograms) based face recognition algorithm and Haar Cascade Classifier for face detection. The project consists of three main parts: face dataset collection, training the face recognition model, and real-time face recognition.

## Part 1: Face Dataset Collection (`face_dataset.py`)
- This program is used to collect a face dataset from the camera.
- The user is prompted to input a USER ID for identification.
- The camera starts capturing images and detecting faces.
- Each detected face is saved in the dataset with the format "User.ID.{count}.jpg" in the 'dataset' folder.
- The dataset collection process ends after 30 face images have been successfully captured or can be stopped by pressing the 'Esc' key.

## Part 2: Model Training (`face_training.py`)
- This program is responsible for training the face recognition model using the previously collected dataset.
- The LBPHFaceRecognizer from OpenCV is used as the recognition model.
- The captured face dataset is loaded, and the model is trained with the dataset.
- The trained model is saved in the "trainer.yml" file in the 'trainer' folder.

## Part 3: Face Recognition (`face_recognition.py`)
- This program is used for real-time face recognition using the pre-trained model.
- The trained face recognition model is loaded.
- The camera captures images and detects faces.
- Each detected face is identified using the trained model.
- The name and confidence level of each detected face are displayed on the screen.

## Usage
1. **Preparation:**
    - Make sure Python, OpenCV, and the required libraries are installed on your computer.
    - Download the "haarcascade_frontalface_default.xml" file for face detection.
    - Save the file in the same directory as the Python code.

2. **Running the Code:**
    - Run each Python script in the specified order (face_dataset.py, face_training.py, face_recognition.py).
    - Follow the on-screen instructions for each part of the process.

## Dependencies
- Python 3.x
- OpenCV (cv2)
- NumPy
- PIL (Python Imaging Library)

## References
- OpenCV Documentation: [https://docs.opencv.org/](https://docs.opencv.org/)
- Local Binary Patterns Histograms (LBPH): [https://docs.opencv.org/3.4/da/d60/tutorial_face_main.html](https://docs.opencv.org/3.4/da/d60/tutorial_face_main.html)
- Haar Cascade Classifier: [https://docs.opencv.org/3.4/db/d28/tutorial_cascade_classifier.html](https://docs.opencv.org/3.4/db/d28/tutorial_cascade_classifier.html)
