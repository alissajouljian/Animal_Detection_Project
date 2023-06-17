Code for Animal Classification

This code performs animal classification using a dataset of raw images. It follows the steps below:

Set the directory path for the dataset containing animal images(Animal-10 dataset) 
Define a list of animal classes.
Iterate over each animal class and load the images from their respective directories.
Preprocess the images by resizing them to a target size and converting them to an array.
Store the preprocessed images in the images list and their corresponding labels in the labels list.
Convert the images and label lists into NumPy arrays.
Encode the categorical labels using a LabelEncoder.
Split the dataset into training and testing sets using the train_test_split function.
Normalize the pixel values of the images by dividing them by 255.0.
Convert the categorical labels into one-hot encoded vectors using to_categorical.
Define the input shape and create an input tensor.
Load the pre-trained InceptionV3 model and attach it to the input tensor.
Add additional layers to fine-tune the model for animal classification.
Create a new model with the input tensor and the modified layers.
Freeze the weights of the InceptionV3 model to prevent them from being updated during training.
Compile the model with the Adam optimizer and categorical cross-entropy loss.
Train the model on the training data for a specified number of epochs.
Evaluate the model's performance on the testing data.
