# Facial-Recognition
This repository provides the outline for creating a facial recognition model using a custom VGG CNN Model

# Image Dataset 
- The dataset should be based on the number (N) of individual faces one wishes to uniquely detect
- Each individual (person) would be an unique class and the output shall be a probability value for the input image against each class
- Please ensure that the number of images for each class (individual) is the same and is cropped to the face.
- There sould not be any other face in the images and the faces should be clearly visible
- The dataset is split 80-20 into Train and Test


# Custom VGG Architecture
- Input Shape - 128 x 128
- Convolution Layer (32) 
- Convolution Layer (32)
- Pooling Layer (2x2)
- Convolution Layer (64)
- Convolution Layer (64)
- Pooling Layer (2x2)
- Convolution Layer (128)
- Convolution Layer (128)
- Pooling (2x2)
- Flatten Layer
- FUC (128) Relu
- Output Later (Output - N) (Activation = Softmax; Loss = Categorical Crossentropy; Optimiser = Adam)


# Using the Trained Model
- Use the file  **Model Generator_Facial Recognition_CustomVGG** to train the model on the UKT Image dataset and save the model file (.h5) at a desired location
- Use the file **Video_Facial Recognition_CustomVGG_CNN** by inserting the Model file name and location in order to predict gender with the computer Webcam
