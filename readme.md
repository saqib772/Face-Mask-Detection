# Face Mask Detection using MobileNetV2
This is a Python script for real-time face mask detection using MobileNetV2 and OpenCV. It uses a pre-trained MobileNetV2 model as a feature extractor and a custom trained face mask detection model to classify whether a person is wearing a face mask or not.


## Requirements
Python 3.x
TensorFlow
Keras
OpenCV (cv2)
NumPy
imutils

Install the required packages using the following command:
```
pip install tensorflow keras opencv-python imutils

```
## How to Use
Clone or download the repository to your local machine.
Navigate to the directory containing the face_mask.py script.
Run the script using the following command:

```
python face_mask_detection.py

```
## Description

The script performs real-time face mask detection on the video stream from the default camera (usually the webcam). It uses a pre-trained MobileNetV2 model to detect faces in the video frames and a custom trained face mask detection model to classify whether the detected faces have masks or not.

The detect_and_predict_mask function is responsible for detecting faces in the frame and predicting whether the person is wearing a mask or not. The face detection model used is based on the Single Shot Multibox Detector (SSD) framework with a MobileNetV2 backbone.

The custom trained face mask detection model (maskNet) is loaded using Keras' load_model function.

The script displays the video stream in real-time, with bounding boxes and labels drawn around each detected face indicating whether the person is wearing a mask or not. A green bounding box and label indicate that the person is wearing a mask, while a red bounding box and label indicate that the person is not wearing a mask.

To exit the video stream, press the 'q' key.
