## Chinese Characters Recognition

# Objective

The goal of this project is to build a machine learning model for the classification of handwritten Chinese characters representing numbers. I will be using a dataset called "Handwritten Chinese Numbers" collected by PhD. K Nazarpour and PhD. M Chen from Newcastle University.

# Dataset

Dataset Source: Kaggle - https://www.kaggle.com/datasets/gpreda/chinese-mnist

The dataset consists of handwritten Chinese characters that represent numbers (0-9 and additional characters). The images are in JPEG format, and each image has a size of 64x64 pixels. There are corresponding labels for each character.

# Exploratory Data Analysis

I performed exploratory data analysis to understand the dataset. This included loading the CSV file, checking the distribution of characters, and verifying the integrity of file names.

# Data Preprocessing

I preprocessed the data by converting the images to grayscale and encoding the labels.

# Baseline Model

I built a baseline model using a feedforward neural network with three hidden layers and ReLU activation functions. I initially trained this model for 10 epochs and observed overfitting.
I improved the model's performance by adding dropout layers to mitigate overfitting. The dropout-enhanced model achieved higher accuracy on the test dataset.

# Convolutional Neural Network (CNN)

I implemented a Convolutional Neural Network (CNN) with two convolutional layers, max-pooling layers, and an output layer with softmax activation. The CNN achieved even better accuracy than the baseline model.
I evaluated the final CNN model, achieving an accuracy of 92.5% on the test dataset.

# Further Enhancements

I attempted to further improve the model by adding an additional convolutional layer with 128 filters, but this did not significantly improve performance.
