# Cardiac_Arrhythmia

Introduction

The focus of this project is to classify whether the patient has “normal” or “abnormal” heart sound from the Phonocardiogram (PCG) or heartbeat recordings to quickly identify patients who would require further diagnosis. This is a supervised learning problem since we already know if the heart sound in training dataset is normal or abnormal. The basic idea is to convert each heart sound recording(wav file) to a spectrogram image and train a Convolutional Neural Network over those images. Then given a new PCG recording, we will be able to classify it as normal or abnormal.

The model (Convolutional Neural Network) takes images as input. So we first need to convert the recordings into spectrogram images. This is taken care by 'spec.py'. The dataset used for this capstone is available freely as part of the PhysioNet / Computing in Cardiology Challenge 2016 which focuses on automatic classification of normal / abnormal phonocardiogram (PCG) recording. Along with clean heart sounds, the dataset also contains some noisy recordings. The samples have been obtained from both normal subjects and pathological patients, providing a variety of signal sources.

Dataset

The heartbeat recording can be downloaded from "https://physionet.org/physiobank/database/challenge/2016/". The dataset contains about 3500 recording but we will only use about 1000 due to memory and computation constraints. After converting the .wav recordings into spectrogram images, the training dataset has 800 images (of which 400 belong to abnormal and 600 to normal class) and test set contains around 225 images(80 of abnormal and rest belong to normal class).

Reqiurements

This project requires Python 3 and the following Python libraries installed:

Keras
Tensorflow
Numpy
Scipy
Matplotlib

You will also need to have software installed to run and execute a Jupyter Notebook

You could just install Anaconda distribution of Python, which already has the above packages and more included.

