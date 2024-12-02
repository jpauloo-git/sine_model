# Sine Wave Regression Using TensorFlow  

This repository contains a Python script designed for Google Colab that demonstrates a complete machine learning pipeline for modeling a noisy sine wave. The script leverages TensorFlow, Keras, and NumPy to create, train, and export a neural network model for regression.  

## Features  

### 1. Dataset Generation  
- Generates a synthetic dataset with `nsamples` points.  
- Creates a noisy sine wave using the equation: `y = sin(x) + noise`.  
- Splits the dataset into training, validation, and test sets.  

### 2. Model Architecture  
- Utilizes a Sequential model with:  
  - Two hidden layers, each with 16 neurons and ReLU activation.  
  - One output layer producing a single scalar prediction.  

### 3. Training and Validation  
- Optimized with the RMSprop optimizer.  
- Uses Mean Absolute Error (MAE) as the loss metric.  
- Monitors training and validation losses during the training process.  

### 4. Visualization  
- Provides graphical plots for:  
  - Dataset and its splits (training, validation, and test sets).  
  - Training and validation loss trends over epochs.  
  - Predictions compared to actual test values.  

### 5. Model Export  
- Converts the trained Keras model into TensorFlow Lite format (`.tflite`) for deployment.  
- Saves both `.tflite` and `.h5` versions of the model.  

## Requirements  

- Python 3.x  
- TensorFlow 2.x  
- NumPy  
- Matplotlib  

## How to Use  

1. Clone the repository:  
   ```bash  
   git clone <repository_url>  
   cd <repository_folder>  
