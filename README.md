# Face-recognition-using-CNN-Deep-Learning

### This project implements a face recognition system using Convolutional Neural Networks (CNN) and OpenCV. The model is trained to recognize faces from a given dataset and can identify individuals

## Table of Contents
- Overview
-  Installation
- Usage
- Project Structure
- Contributing

## Overview
### The project consists of four main components:

- Dataset Generation: Capture images from a webcam and save them for training.
- Data Preparation: Load images, preprocess them, and create training and testing datasets.
- Model Training: Build and train a CNN model to recognize faces.
- Live Face Recognition: Use the trained model to recognize faces in real-time through a webcam 
  feed.
## Installation
### To set up the project, you need to install the following dependencies:

```
pip install opencv-python numpy tensorflow tqdm
```

You will also need to download the haarcascade_frontalface_default.xml file, which can be obtained from OpenCV's GitHub repository.

## Usage
1. Generate the Dataset: Run the generate_dataset.py script to capture images from your webcam.
```
python generate_dataset.py
```
This script will create a folder named data/ containing the captured images.

2. Prepare the Data: Run the prepare_data.py script to preprocess the images and split them 
   into training and testing sets.
```
python prepare_data.py
```
3. Train the Model: Execute the train_model.py script to build and train the CNN model.
```
python train_model.py
```
4. Live Face Recognition: Use the live_face_recognition.py script to start recognizing faces in 
   real-time.

```
python live_face_recognition.py
```
Project Structure
```
FaceRecognitionModel/
│
├── data/                          # Folder to store captured images
│   ├── yourimage.1.jpg
│   ├── yourimage.2.jpg
│   └── ...
│
├── haarcascade_frontalface_default.xml # Haarcascade for face detection
├── generate_dataset.py            # Script to capture images from webcam
├── prepare_data.py                # Script to preprocess images
├── train_model.py                 # Script to train the CNN model
└── live_face_recognition.py       # Script for live face recognition
```
### Contributing
Contributions are welcome! If you have suggestions or improvements, feel free to create an issue or submit a pull request.
