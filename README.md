# Face_Recognization

Face Recognition System
Objective:
To build a Python-based face recognition system using OpenCV and related libraries. It detects and recognizes faces either from images or live video feed.

 Main Components:
Libraries Used:
cv2 (OpenCV) – for image processing and face detection.

os – to handle directories and files.

numpy – for array manipulation.

PIL (Python Imaging Library) – for image handling.

pickle – to serialize and deserialize Python objects.

Steps Implemented:
📌 1. Collecting Training Data
Images are stored in folders labeled with the person's name.

Each person's images are collected and labeled.

📌 2. Face Detection and Feature Extraction
Haar Cascade Classifier is used for face detection (haarcascade_frontalface_default.xml).

Detected faces are extracted and stored with corresponding labels.

📌 3. Training the Recognizer
OpenCV's cv2.face.LBPHFaceRecognizer_create() is used to train the model.

Model and label mappings are saved using pickle and cv2.face.

📌 4. Face Recognition from Live Feed
The model is loaded and run on live webcam feed.

Detected faces are matched with known labels and displayed with names.

📦 Outputs:
A trained model (trainer.yml).

A labels dictionary (labels.pickle).

Live recognition with labeled boxes around recognized faces.

📈 Potential Improvements:
Add more images per person to improve accuracy.

Use a deep learning-based recognizer like FaceNet or Dlib for higher accuracy.

Add GUI for easier interaction.
