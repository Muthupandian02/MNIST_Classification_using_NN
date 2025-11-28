Project Description: MNIST Digit Classification

Overview
This project focuses on building and evaluating machine learning models to classify handwritten digits (0–9) using the **MNIST dataset**. The dataset contains **70,000 grayscale images** of handwritten digits, each sized **28×28 pixels**, split into **60,000 training** and **10,000 testing** samples. MNIST is widely regarded as the “Hello World” of computer vision and serves as a benchmark for image classification tasks.

Objectives
- Preprocess and normalize the MNIST dataset for efficient training.
- Build a **Neural Network (NN)** or **Convolutional Neural Network (CNN)** to classify digits.
- Evaluate model performance using accuracy, confusion matrix, and loss curves.
- Visualize predictions and misclassifications for interpretability.
- Provide a reproducible pipeline for digit recognition tasks.

Methodology
Data Loading 
   - Import MNIST dataset from `tensorflow.keras.datasets` or `sklearn.datasets`.  
   - Split into training and testing sets.

Preprocessing
   - Normalize pixel values (0–255 → 0–1).  
   - Reshape images into vectors (for NN) or retain 2D structure (for CNN).  
   - One-hot encode labels (0–9).

*Model Development
   - **Option A: Fully Connected Neural Network (MLP)**  
     - Input layer: 784 neurons (28×28 pixels).  
     - Hidden layers with ReLU activation.  
     - Output layer: 10 neurons with softmax.  
   - **Option B: Convolutional Neural Network (CNN)**  
     - Convolution + pooling layers for feature extraction.  
     - Dense layers for classification.

Training 
   - Use cross-entropy loss and Adam optimizer.  
   - Train for multiple epochs with batch size tuning.  
   - Monitor training/validation accuracy.

Evaluation 
   - Test accuracy on unseen data.  
   - Confusion matrix to analyze per-digit performance.  
   - Visualize correctly and incorrectly classified digits.

Expected Results
- Achieve **>97% accuracy** with a simple NN.  
- Achieve **>99% accuracy** with a CNN.  
- Provide visualizations of predictions, loss/accuracy curves, and misclassified digits.  

