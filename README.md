# FaceDetection-using-OpenCV
### Identify and recognize a person in the live real-time video.

In this deep learning project, we will learn how to recognize the human faces in live video with Python. We will build this project using python dlib’s facial recognition network. Dlib is a general-purpose software library. Using dlib toolkit, we can make real-world machine learning applications.

### About dlib’s Face Recognition:
Python provides face_recognition API which is built through dlib’s face recognition algorithms. This face_recognition API allows us to implement face detection, real-time face tracking and face recognition applications.

# Project Prerequisites:
You need to install the dlib library and face_recognition API from PyPI:

pip3 install dlib 
pip3 install face_recognition

## Steps to implement Face Recognition with Python:
We will build this python project in two parts. We will build two different python files for these two parts:

[embedding.py](https://github.com/Richa2310/FaceDetection-using-OpenCV/blob/main/embeddings.ipynb): In this step, we will take images of the person as input. We will make the face embeddings of these images.

[recognition.py](https://github.com/Richa2310/FaceDetection-using-OpenCV/blob/main/recognition%20(1).ipynb): Now, we will recognize that particular person from the camera frame.


# 1. [embedding.py](https://github.com/Richa2310/FaceDetection-using-OpenCV/blob/main/embeddings.ipynb):

To identify the person in a pickle file, take its name and a unique id as input:
name=input("enter name")
ref_id=input("enter id")

## Test Images captured using Live Cam

![alt text](https://github.com/Richa2310/FaceDetection-using-OpenCV/blob/main/img1.jpg?raw=true)
![alt text](https://github.com/Richa2310/FaceDetection-using-OpenCV/blob/main/img2.jpg?raw=true)

# 2. [recognition.py](https://github.com/Richa2310/FaceDetection-using-OpenCV/blob/main/recognition%20(1).ipynb):

Here we will again create person’s embeddings from the camera frame. Then, we will match the new embeddings with stored embeddings from the pickle file. The new embeddings of same person will be close to its embeddings into the vector space. And hence we will be able to recognize the person.
Create two lists, one to store ref_id and other for respective embedding:
Start the webcam to recognize the person:

## Output
![alt text](https://github.com/Richa2310/FaceDetection-using-OpenCV/blob/main/img3.jpg?raw=true)
