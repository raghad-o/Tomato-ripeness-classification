# Tomato Ripeness Classification Using Teachable Machine and TensorFlow

## Project Overview

This project aims to develop an image classification model that can distinguish between ripe and unripe tomatoes using Artificial Intelligence and Computer Vision techniques. This type of AI solution can support smart agriculture applications by assisting farmers in monitoring crop maturity, improving harvesting decisions, and enabling automated sorting and quality control systems.

The model was created using Google Teachable Machine, then exported in TensorFlow → Keras format. A Python script was prepared to load the trained model, process input images, and predict the tomato ripeness class with a confidence score.

---

## Project Steps

### 1. Image Collection and Preparation

Images of tomatoes were collected and organized into two classes based on their ripeness level:

- Ripe tomato
- Unripe tomato

A total of 82 images were collected:

- Ripe tomato: 41 images 
- Unripe tomato: 41 images 

The number of images in both classes was kept equal to create a balanced image collection and reduce the possibility of bias toward one class during model training.

---

### 2. Creating and Training the Model Using Teachable Machine

The collected images were uploaded to **Google Teachable Machine** for training.

The following steps were performed:

1. Created an Image Classification project.
2. Added two classes:
   - Ripe tomato
   - Unripe tomato
3. Uploaded the images into their corresponding classes.
4. Trained the model using the prepared images.
5. Tested the model using new tomato images to evaluate its predictions.

![Teachable Machine1](teachable_machine1.png)
![Teachable Machine2](teachable_machine2.png)

---

### 3. Exporting the Model

After completing the training process, the trained model was exported using:

**TensorFlow → Keras format**

The exported files include:

- `keras_model.h5` (trained model)
- `labels.txt` (class labels)

---

### 4. Python Prediction Script

A Python script was prepared to use the exported model for image classification.

The script performs the following steps:

1. Loads the trained model (`keras_model.h5`).
2. Reads the class labels from `labels.txt`.
3. Preprocesses the input image by resizing it to `224 × 224` pixels and normalizing the pixel values.
4. Passes the processed image to the model for prediction.
5. Displays the predicted class and confidence score.

The script was executed using Google Colab with test tomato images to verify the model predictions.

---

### 5. Prediction Results

The model was tested using two tomato images:

![Prediction Results1](prediction1.png)

Class: Ripe tomato
Confidence Score: 0.9999498


![Prediction Results2](prediction2.png)

Class: Unripe tomato
Confidence Score: 0.9998983

The model successfully classified both images with high confidence.

---

## Applications

This project can be applied in smart agriculture systems, including:

- Automatic tomato ripeness detection.
- Supporting farmers in selecting the suitable harvesting time.
- Automated sorting and quality control in agricultural production.
- Camera-based crop monitoring systems.

---


