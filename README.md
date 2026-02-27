# Student Pass/Fail Prediction using Multilayer Perceptron (MLP)

## Overview

This project implements a Multilayer Perceptron (MLP) neural network to predict whether a student will pass or fail a course based on academic performance indicators. The model was developed as part of the ALDL course assignment.

The prediction is based on the following features:

- Attendance Percentage
- Assignment Marks
- Midterm Score
- Final Exam Preparation Time
- Class Participation

This is a binary classification problem:
- 1 = Pass
- 0 = Fail

---

## Objectives

- Design a suitable MLP architecture
- Implement the model using Python
- Perform data preprocessing and normalization
- Train and evaluate the neural network
- Analyze the effect of hidden neurons and learning rate
- Discuss limitations and improvements

---

## Network Architecture

The proposed neural network structure:

- Input Layer: 5 neurons
- Hidden Layer 1: 8 neurons
- Hidden Layer 2: 4 neurons
- Output Layer: 1 neuron

Activation Functions:
- Hidden Layers: ReLU
- Output Layer: Sigmoid

The output neuron produces a probability value between 0 and 1 representing the likelihood of passing the course.

---

## Dataset

A synthetic dataset was generated using NumPy since no real dataset was provided.

Dataset details:
- 300 student records
- 5 input features
- 1 target variable (Pass/Fail)

The target label is generated based on a rule combining attendance, assignment, and midterm scores.

---

## Data Preprocessing

The following preprocessing steps were applied:

1. Feature Scaling using Min-Max Normalization
2. Train-Test Split (80% training, 20% testing)

Feature scaling ensures stable and faster convergence during training.

---

## Model Implementation

The model was implemented using:

- Python
- Scikit-learn
- Google Colab

MLP configuration:

- hidden_layer_sizes = (8, 4)
- activation = 'relu'
- learning_rate_init = 0.01
- max_iter = 500

---

## Evaluation Metrics

The model was evaluated using:

- Accuracy Score
- Confusion Matrix
- Classification Report (Precision, Recall, F1-Score)

These metrics measure the model’s performance in predicting pass/fail outcomes.

---

## Experimental Analysis

### Effect of Hidden Neurons

Increasing hidden neurons improves model capacity but may lead to overfitting if the dataset is small.

### Effect of Learning Rate

A moderate learning rate (0.01) provides stable training. A high learning rate (0.5) may cause unstable convergence and lower accuracy.

---

## Limitations

1. Overfitting risk due to a small dataset.
2. Low interpretability since MLP acts as a black-box model.

---

## Possible Improvements

- Use Cross-Validation
- Apply Regularization techniques
- Collect real-world student performance data
- Compare with other models, such as Logistic Regression or Random Forest

---

## Project Structure

- notebook.ipynb  -> Google Colab implementation
- report.pdf      -> Technical report
- README.md       -> Project documentation

---

## Author Information

Name: Sojib Chandra Roy  
Department: CSE  
Institution: Daffodil Institute of IT (DIIT)  
