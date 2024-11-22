# Waste Classification for Efficient Sorting

This repository provides a deep learning-based solution for automating waste classification in the Grine-Vachine Waste Treatment Center. The goal is to improve Machine 2's sorting algorithm by implementing computer vision models to classify waste items by type, minimizing manual intervention between two Machines.

## Project Overview

The Grine-Vachine Waste Treatment Center currently relies on manual workers to organize waste before Machine processes it. This project introduces deep learning models to automate the classification and routing of waste items to one of six conveyor belts, significantly reducing the need for manual sorting.

### Objectives

1. **Automate waste classification**: Develop a deep learning-based solution for classifying waste images into predefined categories.
2. **Minimize manual labor**: Allow Machine to route waste items efficiently, reducing the need for human intervention.
3. **Improve sorting accuracy**: Ensure only correctly classified waste items reach Machine for processing.

## Dataset

The project utilizes a dataset of waste images captured by Machine during a typical 10-minute operational window. These images have been manually labeled according to their waste type, representing the usual distribution of waste at the center.

## Notebooks

This project includes three main Jupyter notebooks, each implementing a different deep learning approach for waste classification:

1. **`main_resnet.ipynb`**: Uses a ResNet-based architecture, known for its effectiveness in image classification tasks. ResNet (Residual Networks) helps avoid the vanishing gradient problem, making it a strong choice for deep networks.

2. **`main_transformer.ipynb`**: Implements a Vision Transformer (ViT) model. Transformers, traditionally used in NLP, have been adapted for CV tasks and are effective at capturing image features, especially in cases with abundant data.

3. **`main_cnn.ipynb`**: A custom Convolutional Neural Network (CNN) model designed for this classification task. CNNs are a popular choice for image-based tasks due to their efficiency in feature extraction through convolutional layers.

Each notebook includes code for:

- **Data Loading and Preprocessing**: Loading images, splitting data, and preparing them for model training.
- **Model Architecture**: Defining and compiling the model architecture.
- **Training**: Training the model on the provided dataset, with validation metrics to monitor performance.
- **Evaluation**: Testing the model to assess its accuracy and reliability on unseen data.

## Model Comparison

Each notebook provides a unique approach to waste classification:

- **ResNet**: Deep residual connections enhance performance, particularly on deeper models.
- **Transformer**: Captures global dependencies in images, potentially improving classification accuracy on diverse datasets.
- **CNN**: Lightweight model suitable for environments with limited resources, potentially offering faster inference times.
