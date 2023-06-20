# Skin_cancer_prediction-CNN-LSTM-

The dataset is a large collection of multi-source dermatoscopic images of pigmented lesions.

Steps:
1. Loading the dataset.
2. Mapping the image IDs to their file paths.
3. Preprocessing the metadata.
4. Adding image column to metadata/dataset by first resizing the image and then converting it to array and mapping it to the corresponding file path. column output --> (pixel dimensions)
5. Creating training and testing sets.
6. Performing normalization on both sets with z-score normalization.
7. Creating validation set from the training set.
8. Generating augmented images by applying a variety of random transformations, such as rotations, shifts, flips, zooms, and more, to the original training images. 
   This helps increase the size of the training set and introduces diversity into the data, which can improve the model's ability to generalize and handle variations in the test data.
9. MODEL1- Building a CNN model. The model is a sequential neural network with multiple convolutional layers followed by batch normalization, max pooling, and dropout layers. It ends with a flatten layer and two    dense layers. The final dense layer has 7 output units, indicating a multi-class classification problem with 7 classes.
10. Initializing techniques like learning rate reduction which helps improve the training process and early stopping that helps in preventing overfitting and find the optimal number of training iterations.
11. Training the model with 10 epochs.
12. Monitoring the training process - ploting the training and validation loss as well as the training and validation accuracy over the epochs of a model trained using the Adam optimizer .
13. Model evaluation stats - Validation: accuracy = 0.753117  ;  loss_v = 0.702280
                             Test: accuracy = 0.751872  ;  loss = 0.723343
14. Prediction on the validation set.
15. MODEL2 - Building a CNN+LSTM model. The model2 is a sequential neural network architecture consisting of multiple convolutional layers with batch normalization and max pooling, followed by a combination of       LSTM and dense layers.
16. Plotting the training process over the epochs of model.
17. Evaluation and Prediction on model2. 
