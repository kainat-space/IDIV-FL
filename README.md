# IDIV-FL
Intrusion Detection in In-Vehicle Network using Federated Learning

📘 Overview

This repository presents an implementation of a Federated Learning (FL) framework integrated with a Convolutional Neural Network (CNN) model, trained and evaluated using the CICIoV2024 dataset. The project aims to design a decentralized, privacy-preserving intrusion detection system for Internet of Vehicles (IoV) environments while maintaining high accuracy and robust model performance.

🎯 Objectives

Develop a CNN-based intrusion detection model for IoV network data. Integrate the model within a federated learning framework to preserve data privacy across clients. Evaluate model performance using accuracy, precision, recall, F1-score, and AUC metrics. Compare results for both binary and multi-class classification scenarios.

⚙️ Federated Learning Configuration

The federated setup follows TensorFlow Federated (TFF) architecture with the following steps:

  * Model Initialization – The global CNN model is defined and broadcast to all clients.
  * Local Training – Each client trains its local CNN model using private data.
  * Model Aggregation – Local weights are securely aggregated on the central server.
  * Global Update – The updated global model is redistributed to clients.
  * Iteration – Steps 2–4 repeat for multiple rounds until convergence.

🧪 Dataset: CICIoV2024

The CICIoV2024 dataset is a recent and comprehensive dataset for intrusion detection in intra-vehicle networks. It contains labeled CAN-bus traffic data representing normal and attack patterns across multiple vehicle ECUs.

📊 Evaluation Metrics

The model performance is evaluated using:

  * Accuracy
  * Precision
  * Recall
  * F1-Score
  * Confusion Matrix
  * AUC Curve (Area Under ROC Curve)

Both binary and multi-class classification settings are supported.
