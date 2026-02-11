# Intrusion Detection System Using CNN-LSTM

This project implements a CNN-LSTM-based Intrusion Detection System (IDS) for network traffic data. The model is designed to 
detect malicious activities in network environments by leveraging both local feature extraction and sequential pattern learning.

# Overview

Cybersecurity threats are increasingly sophisticated, making Intrusion Detection Systems (IDS) critical for monitoring network 
traffic and preventing attacks. This project applies deep learning techniques, combining Convolutional Neural Networks (CNNs) and 
Long Short-Term Memory (LSTM) networks to effectively detect intrusions in real-time network traffic.

1- Dataset & Preprocessing: Before feeding the data into the model, the following preprocessing steps were performed:
- Data Cleaning: Removed irrelevant or redundant features.
- Scaling: Normalized numerical features to ensure consistent magnitudes.
- One-Hot Encoding: Converted categorical features into binary vectors.
- SMOTE (Synthetic Minority Oversampling Technique): Addressed class imbalance by generating synthetic samples for minority classes.
These steps ensure the model can learn effectively from both the numeric and categorical aspects of network traffic data.

2- Model Architecture
The CNN-LSTM architecture is designed to capture both local patterns and temporal dependencies in network traffic:
- Convolutional Layer (Conv1D): Extracts local features from the input sequences.
- MaxPooling Layer: Reduces dimensionality of feature maps while retaining important features.
- LSTM Layers: Captures sequential dependencies and patterns essential for detecting anomalies in network traffic.
- Dropout Layers: Prevents overfitting by randomly disabling a fraction of neurons during training.
- Dense Layers: Fully connected layers that map learned features to the final output classes.
The combination of CNN and LSTM allows the model to simultaneously learn spatial and temporal characteristics of the data.

3- Training & Evaluation
- Metrics: Accuracy, Precision, Recall, F1-score

# Usage
- Clone the repository: git clone https://github.com/your-username/ids-cnn-lstm.git
- Install required libraries: pip install -r requirements.txt
