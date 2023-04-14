# Car Brand Recognition using HoG Features and Deep Learning

This project is about recognizing car brand logos using HoG features and deep learning. 

# Requirements

To run this project, you need to have the following libraries installed:

    scikit-image
    matplotlib
    OpenCV
    NumPy
    scikit-learn
    TensorFlow
    
# Implementation Details

- The images are read using OpenCV and converted to grayscale.
- Each image is resized to 128 x 128 pixels.
- HoG features are extracted from each image using scikit-image's hog function.
- The orientation is set to 9, and the pixels per cell and cells per block are set to (8, 8) and (2, 2), respectively.
- The features and the labels are stored in two separate lists.
- The features and labels are converted to NumPy arrays.
- The dataset is split into training and testing sets using scikit-learn's train_test_split function.
- A deep learning model is created using TensorFlow's Keras API.
- The model has one hidden layer with 1000 units and a sigmoid activation function.
- The output layer has three units, one for each brand, and a softmax activation function.
- The model is trained using the Adam optimizer and the sparse categorical cross-entropy loss function.
- The accuracy of the model is calculated on the testing set.

# Tests
![Tesla%20Test%20Result%202.png](https://github.com/TianjianNi/Car-Brand-Logo-Recognition-using-HoG-Features-and-Deep-Learning/blob/main/Test%20Result/Tesla%20Test%20Result%202.png)
![Tesla%20Test%20Result%201.png](https://github.com/TianjianNi/Car-Brand-Logo-Recognition-using-HoG-Features-and-Deep-Learning/blob/main/Test%20Result/Tesla%20Test%20Result%201.png)
![BMW%20Test%20Result1.png](https://github.com/TianjianNi/Car-Brand-Logo-Recognition-using-HoG-Features-and-Deep-Learning/blob/main/Test%20Result/BMW%20Test%20Result1.png)
![BMW%20Test%20Result2.png](https://github.com/TianjianNi/Car-Brand-Logo-Recognition-using-HoG-Features-and-Deep-Learning/blob/main/Test%20Result/BMW%20Test%20Result2.png)
![Benz%20Test%20Result%201.png](https://github.com/TianjianNi/Car-Brand-Logo-Recognition-using-HoG-Features-and-Deep-Learning/blob/main/Test%20Result/Benz%20Test%20Result%201.png)
![Benz%20Test%20Result%203.png](https://github.com/TianjianNi/Car-Brand-Logo-Recognition-using-HoG-Features-and-Deep-Learning/blob/main/Test%20Result/Benz%20Test%20Result%203.png)

# Results

The model achieves an accuracy of 91.67% on the testing set after 20 epochs.
