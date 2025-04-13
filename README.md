# Image Classification with Keras
A deep learning project for image classification using TensorFlow/Keras, featuring model checkpointing and validation monitoring.

 ## 📌 Overview
This project implements an image classification model using TensorFlow/Keras, with a focus on:

Training a CNN (Convolutional Neural Network) for image recognition.

Saving the best model using ModelCheckpoint based on validation accuracy.

Analyzing training dynamics (e.g., fluctuating training accuracy vs. stagnant validation accuracy).

## 🔍 Key Observations During Training:

Validation accuracy remained constant (~66.63%) while training accuracy varied significantly (59%–87%).

Possible issues: overfitting, insufficient model capacity, or data imbalance.

Next steps: Hyperparameter tuning, data augmentation, or architecture changes to improve generalization.

## 🛠️ Installation & Setup

Clone the repository: git clone https://github.com/Anusuyakashyap/Final-year-project.git
cd your-repo

Install dependencies: pip install tensorflow numpy matplotlib

Run the training script: python train.py

##  Project Structure
├── data/                    # Training/validation datasets
├── models/                  # Saved models (e.g., best_model.keras)
├── train.py                 # Training script with ModelCheckpoint
├── utils/                   # Helper functions (data loading, preprocessing)
└── README.md

## Hyperparameters & Training
Epochs: 30
Callbacks: ModelCheckpoint('best_model.keras', monitor='val_accuracy', save_best_only=True, mode='max')
Metrics Tracked: Training/Validation Accuracy,Training/Validation Loss

## Performance Insights
![Screenshot (50)](https://github.com/user-attachments/assets/f0339e96-ffc7-46be-8e6f-6776ea4f0707)

![Screenshot 2025-04-13 211342](https://github.com/user-attachments/assets/6644ce30-94ea-4d32-9584-839c89cefa59)

![Screenshot (52)](https://github.com/user-attachments/assets/a509be25-7432-45a8-b97a-9b9ffbf0a924)

  ## Next Steps
  Data Augmentation (e.g., ImageDataGenerator) to improve generalization.
  Learning Rate Scheduling (ReduceLROnPlateau) for better convergence.
  Model Architecture Changes (deeper CNN, transfer learning).
