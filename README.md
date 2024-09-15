# English-Thai and Thai-English Translation Project

This project is an English-to-Thai and Thai-to-English translation system based on a custom-trained machine learning model. The model can translate simple sentences effectively but struggles with more complex sentences due to limited training. The project allows users to choose the translation direction with an optional input: `[1 for EN-TH, 2 for TH-EN]`.

## Overview

- **Objective**: To develop a translation system capable of translating text between English and Thai.
- **Current Capabilities**: The model can handle simple sentences and common phrases but may have issues with complex sentences and idiomatic expressions.
- **Model Training**: The model has been trained four times using checkpoints to save progress, with simplified training settings due to resource limitations.

## Features

- **Translation Directions**:
- `1` for English-to-Thai (EN-TH)
- `2` for Thai-to-English (TH-EN)
- **Simple Sentence Translation**: Suitable for basic and straightforward sentences.
- **Custom-Trained Model**: Built using deep learning techniques tailored to English-Thai language pairs.

## Files in This Project

**CapstoneProject_Group10.ipynb**: A Jupyter notebook that contains the code for preprocessing the data, training the translation model, and evaluating its performance. This notebook demonstrates the steps taken to build and test the translation model.

## Usage
- **Input**: Enter a sentence in either English or Thai.
- **Option**: Choose the translation direction [1 for EN-TH, 2 for TH-EN].
- **Output**: The translated sentence will be displayed based on the selected direction.

## Model Training Details
- **Training Process**: The model was trained in four separate runs using checkpoints to save progress, allowing for iterative improvements without starting from scratch.
- **Simplified Training Settings**: Due to limited computational resources, the model was trained with basic settings. This was done to optimize training time while demonstrating the core concept of machine translation between English and Thai.
- **Improvement Opportunities**: For better results, consider expanding the dataset, adjusting hyperparameters, and increasing computational resources to allow for more complex model architectures.

## Improving the Model
The current model performance can be improved by adjusting the following values and parameters:

- **Training Data Size**: Increasing the size and diversity of the training dataset can significantly enhance the model's ability to handle complex sentences and idiomatic expressions.
- **Batch Size**: Adjusting the batch size (e.g., from 32 to 64 or 128) can impact the speed and quality of training. Larger batch sizes might speed up training but require more memory.
- **Learning Rate**: Tuning the learning rate (e.g., from 0.001 to 0.0001 or 0.01) can help the model converge faster or avoid overshooting the optimal parameters. Experiment with different values to find a suitable balance.
- **Number of Epochs**: Increasing the number of training epochs (e.g., from 10 to 50 or more) allows the model to learn better, but be cautious of overfitting. More epochs may be required if you add more data or adjust other hyperparameters.
- **Model Architecture**: Modifying the neural network architecture (e.g., adding more layers, changing the number of neurons, or incorporating attention mechanisms) can lead to better performance but may also increase training time and computational requirements.
- **Regularization Techniques**: Applying regularization methods (e.g., dropout rate adjustment, weight decay) can prevent overfitting and improve generalization.
- **Data Augmentation**: Implement data augmentation techniques, such as back-translation, to create more varied training samples.

## Limitations
- **Complex Sentences**: The current model after the fourth train may struggle with translating complex sentences or sentences with less common phrases.
- **Resource Constraints**: The training process is optimized for limited computational resources, and improvements may require more powerful hardware.
