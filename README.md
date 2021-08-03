# handwritten_digits_classification

PROBLEM STATEMENT / DESCRIPTION

Writing digits manually and identifying them becomes a huge task when we have heaps of data.
Considering this, there’s significant business and educational interest in developing AI that can recognize handwritten images. Starting off with classification of handwritten digits, we can later implement similar techniques on other types of handwritten data. Initially, for this project we are only dealing with the development of a neural network from scratch for MNIST handwritten digit classification.


DATASET

The MNIST dataset (Modified National Institute of Standard and Technology) is a dataset consisting of 60,000 small scale 28*28 pixel grayscale images of single handwritten digits from 0 to 9.
The objective is to classify these handwritten digits into one of the 10 classes representing values from 0 to 9.
The test dataset consists of 10,000 handwritten images of 28*28 pixel. 
Uniform distribution between train and test dataset.

PREPARING DATASET
Load the dataset from keras.
We know that the pixel values for each image in the dataset are unsigned integers in the range between black and white, 0 to 255. Therefore re-scaling them is necessary for better accuracy.
Reshape the data frame (flatten it).[to feed as input]
Output will have 10 classes 0 to 9.

Model
Initially using a simple neural network with one input layer(784 elements) and an output layer(10 elements). Activation function - sigmoid, metric-accuracy, loss- sparse_categorical_crossentopy. Achieved accuracy of 92% on test images.
Tested on a sample image (7) prediction was correct.
Used hidden layers and model performed significantly well with accuracy of 97% on test images.
