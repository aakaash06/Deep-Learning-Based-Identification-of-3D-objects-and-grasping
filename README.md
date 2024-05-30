# Deep-Learning-Based-Identification-of-3D-objects-and-grasping
Key highlights of the project include:
🔸 Leveraging pre-trained DL network (Generative Grasping Convolutional Neural Network) to accurately identify objects and determine the optimal grasp location.
🔸 Creating a dataset of custom 3D objects.
🔸 Utilizing the results from the DL algorithm to successfully grasp objects.
🔸 Employing Robot Studio as a simulation tool to perform grasping.

Please see the GGCNN repository for the Deep Learning code and setup. Use Jacquard dataset to get best results.

A pre-trained DL model - Generative Grasping convolutional Neural Network was first executed. All the system and software requirements had to be accurately followed as given in instructions to get the output. The model was first tested on Jacquard and Cornell dataset. These datasets were used to train the model.
Follow the instructions in https://github.com/dougsm/ggcnn to do this step.
This network returns grasp rectangles when given a picture.

Then, a kinect camera was used to take pictures of the objects that we want to grasp. For this, the pictures should be similar to jacquard or cornell so that best results are returned. So a white background is fixed and the object kept on top of it. While giving these pictures as an input to the model, it returned grasp rectangles and pixel coordinates of such rectangles on the object.

These pixel coordinates are then converted into real world coordinates by using a custom formula. This coordinates can be given as input to the YuMi robot using which then
