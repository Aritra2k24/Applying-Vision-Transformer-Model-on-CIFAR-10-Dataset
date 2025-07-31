# Applying-Vision-Transformer-Model-on-CIFAR-10-Dataset
Hi,  here I have implemented the Vision Transformer Model on CIFAR-10 Dataset

## Project Overview:-

##  Importing the Libraries :-

1. Pytorch
2. Matplotlib
3. Numpy
4. Torchvision
5. Random


## Loading the CIFAR-10 Dataset :-

Here I load the CIFAR-10 dataset containing 50000 training images and 10000 testing images of 10 different classes.

Creating two Diffrent dataset - Training Dataset and Testing Dataset

## Data Preprocessing :-

 Here I preprocessed the input images by random cropping, flipping and rotating the images so that the model perform unbiased in the spatial changes of the images.

 ## Creating the different parts of the Vision Transformer Model Architecture :-

 1. Patch Embedding Layer :- here I use the Convolution operation on the Images to extract the important features
 2. Transformer Encoder Layer
 3. Multi Layer Perceptron

 now I embedded all these Layers to form the Vision Transformer Model

 ## Feeding of Input Images :-

 Here at first  the input images are passed through the Patch Embedding where the images are convoluted  and then converted them into 1D shape and added positional embeddings and CLS token.

 Then it is passed through the Encoder Layer which consists of Multi-Head Self Attention Layer and Normalization Layer and the Input images are passed through a residual connection (i.e input is added with the output of these layers).

 Then finally it is passed through the Multi- Layer Perceptron to extract more patterns from the images and also to add non-linearity to the model.

 And then finally the Output of the entire model is passed through the Softmax Function to classify the images into 10 classes.

 ## Model Prediction and Evaluation :- 

 Finally the test images are predicted on the trained model and the model is evaluated.

 <img width="1176" height="854" alt="Screenshot 2025-07-31 143833" src="https://github.com/user-attachments/assets/95ca2204-c6a8-4714-82d0-faf7c136399d" />

 ## Plotting the Accuracy :-

 <img width="926" height="747" alt="Screenshot 2025-07-31 144055" src="https://github.com/user-attachments/assets/d0282755-776f-40fd-865b-4ea662f75adb" />

## Predicted Result :-

<img width="1070" height="872" alt="Screenshot 2025-07-31 144318" src="https://github.com/user-attachments/assets/92309b92-2a3d-4d20-87ba-ed0236b47a6d" />

### Model Architecture :-

<img width="850" height="515" alt="Vision Transformer" src="https://github.com/user-attachments/assets/e9b4079b-3c6b-4999-bace-2c0ff25f25f7" />

