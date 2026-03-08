# Hand and Cup Detection using ESP32-CAM

## Project Overview

This project detects hands and paper cups using an ESP32-CAM and a machine learning model trained with Edge Impulse. The goal of the project was to explore how embedded machine learning can be used with microcontrollers for simple object detection tasks.

The trained model runs directly on the ESP32-CAM and performs real-time detection using the camera.

## Hardware Used

* ESP32-CAM
* USB to TTL converter (for uploading code)
* Jumper wires
* Computer for model training and deployment

## Software / Tools

* Edge Impulse
* Arduino IDE

## Data Collection

Images of hands and paper cups were collected using the ESP32-CAM camera.
The pictures were taken in the same environment where the model would later be tested, so that the model could learn from realistic conditions.

The background was present in the images, but it was not labeled as a separate class. Only the objects hand and cup were labeled during training.

## Steps Followed

1. Collected images of hands and paper cups using the ESP32-CAM.
2. Uploaded the dataset to Edge Impulse.
3. Labeled the objects in the images.
4. Trained an object detection model.
5. Exported the trained model for ESP32 deployment.
6. Integrated the model with the ESP32-CAM using Arduino IDE.
7. Tested the detection using the live camera feed.

## How It Works

The ESP32-CAM captures an image frame and passes it to the trained machine learning model.
The model processes the image and determines whether a hand or a cup is present in the frame.

The detection results can be viewed through the serial monitor.

## Applications

* Smart waste detection systems
* Touchless automation systems
* Learning embedded machine learning
* Basic computer vision projects with microcontrollers

## What I Learned

Through this project, I learned:

* How to collect datasets for machine learning
* How to use Edge Impulse to train an object detection model
* Deploying ML models on microcontrollers like ESP32-CAM
* Integrating embedded ML with Arduino code

## Author

Sandhiya Priyadharshini G
