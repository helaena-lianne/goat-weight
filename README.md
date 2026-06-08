# Goat Weight Prediction and Classification Using Deep Learning

## Overview

This project presents a deep learning-based system for goat weight prediction and classification using image data. The study aims to provide a non-invasive, efficient, and automated method for estimating the live weight of goats, reducing the need for traditional manual weighing procedures.

The system utilizes computer vision and convolutional neural network (CNN) architectures to analyze goat images and predict their corresponding weights. In addition, the system can classify goats into predefined weight categories to support livestock management and decision-making.

## Objectives

* Develop a computer vision system capable of estimating goat live weight from images.
* Compare the performance of different deep learning architectures for weight prediction.
* Classify goats into weight categories based on predicted weights.
* Provide a user-friendly platform for image capture and weight estimation.

## Dataset

The dataset consists of goat images collected from various viewpoints under real-world farm conditions. Each image is paired with the corresponding measured live weight of the goat.

### Dataset Features

* Goat images captured using a mobile device.
* Associated live weight measurements.
* One goat breed but multiple ages and body conditions.
* Diverse environmental conditions and image backgrounds.

## Methodology

### Data Collection

Images of goats were collected and labeled with their actual live weights. The collected dataset was then organized and prepared for model training and evaluation.

### Data Preprocessing

The preprocessing stage includes:

* Image resizing and normalization.
* Data cleaning and quality verification.
* Dataset splitting into training, validation, and testing sets.
* Data augmentation to improve model generalization.

### Model Development

The study evaluates two CNN architectures, including:

* ResNet-50
* MobileNetV2

These models extract visual features from goat images and learn the relationship between body appearance and live weight.

### Weight Prediction

Weight estimation is treated as a regression problem where the model predicts a continuous weight value based on the input image.

### Weight Classification

Predicted weights are categorized into predefined weight classes, allowing easier interpretation and practical use in livestock management.

## Evaluation Metrics

### Regression Metrics

The weight prediction models are evaluated using:

* Mean Absolute Error (MAE)
* Mean Squared Error (MSE)
* Coefficient of Determination (R²)

### Classification Metrics

The weight classification component is evaluated using:

* Accuracy
* Precision
* Recall
* F1-Score
* Confusion Matrix

## Technologies Used

### Programming Language

* Python

### Libraries and Frameworks

* TensorFlow
* Keras
* NumPy
* Pandas
* OpenCV
* Matplotlib
* Scikit-learn

### Development Environment

* Google Colab

## Repository Note

This thesis evaluates and compares multiple convolutional neural network architectures, namely ResNet-50 and MobileNetV2, for goat weight prediction and classification. However, this GitHub repository only contains the implementation, training, and evaluation pipeline for the MobileNetV2 model.

The complete thesis manuscript includes the methodology, experimental setup, comparative analysis, and performance results of all evaluated architectures. The MobileNetV2 implementation is provided in this repository as a reproducible version of the developed system.

### Evaluation

Evaluate the trained model using the provided testing dataset to generate regression and classification performance metrics.

### Prediction

Provide a goat image to the trained model to obtain:

* Predicted live weight
* Corresponding weight category (small, medium, and large)

## Results

The developed models demonstrate the feasibility of using computer vision and deep learning techniques for estimating goat live weight from images. The study highlights both the potential and challenges of image-based livestock weight estimation.

Experimental results indicate that model performance is influenced by several factors, including dataset size, image quality, viewing angles, lighting conditions, and the distribution of goat weights within the dataset. The findings provide valuable insights for future research in precision livestock farming and agricultural artificial intelligence applications.

## Limitations

* Limited dataset size compared to large-scale computer vision datasets.
* Variations in image quality and environmental conditions.
* Inconsistent image angles may affect prediction accuracy.
* Dataset imbalance across weight ranges may influence model performance.

## Future Work

* Expand the dataset with additional goat images and breeds.
* Collect standardized images from multiple viewpoints.
* Investigate advanced architectures and ensemble approaches.
* Improve weight classification performance.
* Deploy the system as a mobile or web-based application for real-time use.
* Extend the framework to other livestock species.

## Researchers

This project was developed as part of an undergraduate thesis in Data Science at Ateneo de Davao University.

## Acknowledgments

The researchers would like to thank the participating farms, data collectors, advisers, and institutions that supported the development of this study.

## Disclaimer

This project was developed for research and educational purposes. The predicted weights should be considered estimations and should complement, rather than replace, standard livestock weighing procedures in professional agricultural settings.
