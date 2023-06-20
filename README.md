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
9. 
