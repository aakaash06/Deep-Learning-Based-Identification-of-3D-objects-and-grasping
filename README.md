# Deep-Learning-Based-Identification-of-3D-objects-and-grasping
This repository contains the code and documentation for a deep learning project aimed at identifying 3D objects and determining optimal grasp locations using a pre-trained Generative Grasping Convolutional Neural Network (GGCNN). The project involves creating a custom dataset of 3D objects, utilizing the GGCNN model to generate grasp coordinates, and employing Robot Studio to simulate and execute the grasping process with a YuMi robot.

Introduction
This project demonstrates the application of a pre-trained deep learning model to identify 3D objects and determine the optimal grasping points. By leveraging the Generative Grasping Convolutional Neural Network (GGCNN), we can accurately predict grasp rectangles for various objects. The project involves creating a custom dataset of 3D objects, capturing images using a Kinect camera, transforming pixel coordinates to real-world coordinates, and simulating the grasping process with Robot Studio.

Dataset
For training and testing the GGCNN model, the Jacquard and Cornell datasets were used. These datasets contain annotated images of objects with labeled grasp rectangles.

Follow the instructions in the GGCNN repository (https://github.com/dougsm/ggcnn) to set up the model and use these datasets effectively.

Pre-trained Model
The project utilizes a pre-trained Generative Grasping Convolutional Neural Network (GGCNN) to predict grasp rectangles. Ensure all system and software requirements are met as specified in the GGCNN repository.

Image Capture
A Kinect camera is used to capture images of the objects to be grasped. To achieve optimal results, ensure that the images have a similar setup to the Jacquard or Cornell datasets, such as a white background with the object placed on top.

Coordinate Transformation
The grasp rectangles returned by the GGCNN model are in pixel coordinates. These coordinates need to be converted into real-world coordinates using a custom formula. The transformed coordinates can then be used as input for the YuMi robot through socket communication, allowing the robot to grasp the object accurately.

Robot Simulation
Robot Studio is employed as a simulation tool to perform the grasping tasks. By using the real-world coordinates obtained from the GGCNN model, the YuMi robot can be programmed to execute precise grasping actions.

We welcome contributions to this project! If you have any ideas, suggestions, or bug fixes, please open an issue or submit a pull request.
