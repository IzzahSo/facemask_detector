# facemask_detector

Face masks are crucial in minimizing the propagation of Covid-19, and are highly recommended, even becoming obligatory in many situations. Due to the outbreak of Covid-19, we propose a system that can therefore be used in real-time applications including easy deployment into existing systems to detect whether the public wear face masks or not. In addition, the system also could be integrated with embedded systems for applications in places to ensure the public safety guidelines are followed.

The Face Mask Recognition System is built with a very simple and basic Convolutional Neural Network (CNN) model using TensorFlow with Keras library and OpenCV to detect if you are wearing a face mask or not. The proposed system is also deployed using Deep Learning and Computer Vision concepts to detect face masks in static images as well as in real-time video streams


# Datasets
The datasets total images is 2410 images. This dataset is divided into two files: _with_mask_ and _without_mask_ with 1210 and 1200 images respectively.

Retrieved here: https://drive.google.com/drive/folders/1tMNKupUjDAJh7hpW_J3x49ADyBcC_O_3?usp=sharing

# System Requirements
The system requirement is as follows:
tensorflow >= 1.15.2
keras == 2.3.1
imutils == 0.5.3
numpy == 1.18.2
opencv-python ==  4.2.0.*
matplotlib == 3.2.1
scipy == 1.4.1

# System Design
In order to train a custom face mask detector, the project is divided into 2 distinct phases, each with its own respective sub-steps

PHASES 
- Training
Datasets are loaded from disk to face mask detection which will be used to train a model using Keras/TensorFlow on these datasets, and then serializing the face mask detector to disk.

- Deployment
Once the face mask detector is trained, the mask detector will load and perform the face detection which then be classified each face as with_mask or without_mask. 

