# Smile-To-Click

The idea of this project is to have a trained model able to detect smiles, that can be used as a trigger when taking selfies.

I already built and trained a convolutional neural network to detect facial keypoints in my previous Udacity's Computer Vision Nanodegree program (archive added to this repo). This model will rake as an input any image with faces and will predict the location of 68 distinguishing keypoints on each face. Facial keypoints include points around the eyes, nose, and mouth on a face and can be used, in conjunction with a facial filter, to detect smiles on faces.

The next steps will be to:
- import the pre-trained model into the OpenVINO tool
- run the model optimizer to make it feasible for using on a smartphone
-  deply the model as an Edge app

When the selfie camera is turned on, the app will start making inference of the image frames, and when a smile is detected (with the options of one face or all faces), the camera shutter is activated.
