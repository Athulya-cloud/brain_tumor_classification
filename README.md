
# A Deep Learning based Medical Imaging Toolkit for Brain Tumor Classification and Detection

This project focuses on classifying and detecting brain tumors using deep learning techniques. It is implemented using Python and various libraries, including TensorFlow and Keras.


## Authors

- [@athulya](https://github.com/Athulya-cloud)
- [@joshin](https://github.com/JoshinAji)
- [@aaron](https://github.com/ajvarghese)

## 🔗 Links

[![linkedin](https://img.shields.io/badge/linkedin-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/athulya-/)










## Table of Contents

- [Data Collection](#data-collection)
- [Data Preprocessing](#data-preprocessing)
- [Model Training](#model-training)
- [Flask Implementation](#flask-implementation)

## Data Collection

The dataset for this project is organized into the following categories:
- `no`: Images without brain tumors.
- `yes/pituitary_tumor`: Images with pituitary brain tumors.
- `yes/meningioma_tumor`: Images with meningioma brain tumors.

## Data Preprocessing

- The images are resized to a common input size of 64x64 pixels.
- Data is split into training and testing sets.
- Image data is normalized for model input.
- Labels are one-hot encoded for multi-class classification (4 classes).

## Model Training

- A Convolutional Neural Network (CNN) model is built using Keras.
- The model consists of Conv2D layers with 'relu' activation functions, max-pooling layers, and dropout layers to prevent overfitting.
- The last layer is a Dense layer with 'softmax' activation for multi-class classification.
- The model is trained using the categorical cross-entropy loss and the Adam optimizer.
- Training is done for 80 epochs with a batch size of 8.

## Flask Implementation

A Flask web application is provided for model testing and predictions.
- The trained model is loaded.
- Users can upload an image for prediction.
- The model predicts whether the uploaded image contains a brain tumor and, if present, classifies the type of tumor.

## Usage

1. Install the required libraries by running `pip install -r requirements.txt`.
2. Run the Flask application: `python app.py`.

Your web application will be available at `http://127.0.0.1:5000/`.



