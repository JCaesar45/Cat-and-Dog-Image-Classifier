# Cat and Dog Image Classifier README

## Project Overview

This project involves building an image classification model to differentiate between images of cats and dogs using TensorFlow 2.0 and Keras. You will work on this project using Google Colaboratory (Colab).

## Getting Started

1. **Create a Google Colaboratory Notebook:**
   - Go to the provided [Google Colaboratory link](#) to access the notebook.
   - Create a copy of the notebook in your Google Drive or download it to run locally.

2. **Preparation:**
   - Ensure that you have access to the TensorFlow library and that you are using at least version 2.0.
   - Familiarize yourself with the dataset structure, which consists of directories for training, validation, and testing images.

   ```
   cats_and_dogs
   ├── train
   │   ├── cats: [cat.0.jpg, cat.1.jpg ...]
   │   └── dogs: [dog.0.jpg, dog.1.jpg ...]
   ├── validation
   │   ├── cats: [cat.2000.jpg, cat.2001.jpg ...]
   │   └── dogs: [dog.2000.jpg, dog.2001.jpg ...]
   └── test: [1.jpg, 2.jpg ...]
   ```

## Instructions

### Cell Structure

- **Cell 1: Import Libraries**
   - Import the necessary libraries required for image classification, including TensorFlow and Keras.

- **Cell 2: Download Data & Set Variables**
   - Download the dataset and set any key variables needed for the project.

- **Cell 3: Create Image Generators**
   - Fill in the variables to create image generators for the training, validation, and test datasets. Use `ImageDataGenerator` to rescale the image tensors.
   - Make sure to use the `flow_from_directory` method correctly for each dataset, especially for the test data, where you need to set `shuffle=False`.

- **Cell 4: Visualizing Images**
   - The function `plotImages` is provided to visualize the images from the training dataset. Running this cell will plot five random training images.

- **Cell 5: Data Augmentation**
   - Recreate the image generator for training data by implementing random transformations to augment the data. This step helps to reduce the risk of overfitting.

- **Cell 6: Verify Data Augmentation**
   - This cell will plot a single image from the training dataset with different augmentations applied.

- **Cell 7: Build the Model**
   - Create a Sequential model using Keras. Design a convolutional neural network (CNN) that includes multiple `Conv2D` and `MaxPooling2D` layers, followed by a fully connected layer with a ReLU activation function.

- **Cell 8: Train the Model**
   - Train your model using the `fit` method. Ensure you pass in the relevant parameters like `steps_per_epoch`, `epochs`, and validation data.

- **Cell 9: Visualize Training Results**
   - Run the model's accuracy and loss visualization to analyze its performance during training.

- **Cell 10: Make Predictions**
   - Use the trained model to predict whether the test images are cats or dogs. Collect the probabilities and visualize them using the `plotImages` function.

- **Cell 11: Submission Check**
   - Finally, check if your project meets the challenge requirements and if your model achieves at least 63% classification accuracy.

## Submission

Once you have completed the project and verified that it passes all tests:
- Submit your project link below.
- For Google Colaboratory submissions, ensure that you enable link sharing for "anyone with the link."

## Additional Resources

Since the interactive instructional content is still being developed, you may need to seek extra learning materials for deeper understanding. Recommended resources may include:
- TensorFlow Documentation
- Keras Documentation
- Online courses (Coursera, Udacity, etc.)

## Acknowledgments

This project aims to refine your skills and provide hands-on experience with image classification using deep learning techniques. Best of luck, and happy coding!
