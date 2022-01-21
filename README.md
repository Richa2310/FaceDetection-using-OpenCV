# FaceDetection-using-OpenCV

Recognize and manipulate faces from Python or from the command line with the world's simplest face recognition library.

Built using dlib's state-of-the-art face recognition built with deep learning. The model has an accuracy of 99.38% on the Labeled Faces in the Wild benchmark.

This also provides a simple face_recognition command line tool that lets you do face recognition on a folder of images from the command line!

## Features
#### Find faces in pictures.
#### Find all the faces that appear in a picture:

## Face Recognition with Python – 
#### Identify and recognize a person in the live real-time video.

In this deep learning project, we will learn how to recognize the human faces in live video with Python. We will build this project using python dlib’s facial recognition network. Dlib is a general-purpose software library. Using dlib toolkit, we can make real-world machine learning applications.

In this project, we will first understand the working of face recognizer. Then we will build face recognition with Python.

## About dlib’s Face Recognition:
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

First, create a file embedding.py in your working directory. In this file, we will create face embeddings of a particular human face. We make face embeddings using face_recognition.face_encodings method. These face embeddings are a 128 dimensional vector. In this vector space, different vectors of same person images are near to each other. After making face embedding, we will store them in a pickle file.

To identify the person in a pickle file, take its name and a unique id as input:
name=input("enter name")
ref_id=input("enter id")

Create a pickle file and dictionary to store face encodings:
Open webcam and 5 photos of a person as input and create its embeddings:
To capture images, press ‘s’ five times. If you want to stop the camera press ‘q’:

Update the pickle file with the face embedding.

# 2. [recognition.py](https://github.com/Richa2310/FaceDetection-using-OpenCV/blob/main/recognition%20(1).ipynb):

Here we will again create person’s embeddings from the camera frame. Then, we will match the new embeddings with stored embeddings from the pickle file. The new embeddings of same person will be close to its embeddings into the vector space. And hence we will be able to recognize the person.
Create two lists, one to store ref_id and other for respective embedding:
Start the webcam to recognize the person:


# Summary:
This deep learning project teaches you how to develop human face recognition project with python libraries dlib and face_recognition APIs (of OpenCV).
