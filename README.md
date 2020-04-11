# Gesture Recognition
A neural network based model for identifying 5 different types of gestures which can be installed on Smart TV Cameras.

#### -- Project Status: [Completed]

## Project Intro/Objective
The goal is to develop a cool feature in the smart-TV that can recognise five different gestures performed by the user which will help users control the TV without using a remote.

### Partner
* Swayam Nanda
* EMail: nanda.swayam@gmail.com

### Methods Used
* Neural Networks
* CNNs, RNNs
* Transfer Learning
* Machine Learning

### Technologies
* Python
* Pandas, jupyter
* skImage

## Project Description
* The gestures are continuously monitored by the webcam mounted on the TV. Each gesture corresponds to a specific command:
   - Thumbs up:  Increase the volume
   - Thumbs down: Decrease the volume
   - Left swipe: 'Jump' backwards 10 seconds
   - Right swipe: 'Jump' forward 10 seconds  
   - Stop: Pause the movie
  
* The training data consists of a few hundred videos categorised into one of the five classes. Each video (typically 2-3 seconds long) is divided into a sequence of 30 frames(images). These videos have been recorded by various people performing one of the five gestures in front of a webcam - similar to what the smart TV will use.

* The data is in a zip file. The zip file contains a 'train' and a 'val' folder with two CSV files for the two folders. These folders are in turn divided into subfolders where each subfolder represents a video of a particular gesture. Each subfolder, i.e. a video, contains 30 frames (or images). Note that all images in a particular video subfolder have the same dimensions but different videos may have different dimensions. Specifically, videos have two types of dimensions - either 360x360 or 120x160 (depending on the webcam used to record the videos). Hence, you will need to do some pre-processing to standardise the videos. 

* Each row of the CSV file represents one video and contains three main pieces of information - the name of the subfolder containing the 30 images of the video, the name of the gesture and the numeric label (between 0-4) of the video.

* Two common proven network architecture for gesture recognition
   * Convolutions + RNN - The conv2D network will extract a feature vector for each image, and a sequence of these feature vectors is then fed to an RNN-based network. The output of the RNN is a regular softmax (for a classification problem such as this one).
   * 3D Convolutional Network, or Conv3D - 3D convolutions are a natural extension to the 2D convolutions

## Getting Started

1. Clone this repo (for help see this [tutorial](https://help.github.com/articles/cloning-a-repository/)).
2. Raw Data is being kept [https://drive.google.com/drive/folders/1VxhQI8c3hHiWdstJeIJ_opbX3l7eSei9?usp=sharing](train & val folder containing videos, train.csv and val.csv containing gesture frames path and type of gesture) within this repo.

## Contact
Shubham Patel
shubhampatel1608@gmail.com
Mobile: 8103856241
