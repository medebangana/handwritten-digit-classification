# Handwritten Digit Classification using CNN & RNN
A deep learning project for handwritten digit classification using the MNIST dataset and PyTorch. The project implements both a Convolutional Neural Network (CNN) and a Recurrent Neural Network (RNN) and compares their performance on the same classification task.

# 📊 Dataset
Dataset: MNIST
60,000 training images
10,000 test images
Image size: 28 × 28 pixels
Grayscale images
10 classes: digits 0–9

Images were converted to tensors and normalized before training.

# Models
## CNN

The CNN learns spatial features from the handwritten images using:

Convolutional layers - 
ReLU activation - 
Max pooling - 
Fully connected layers - 
10-class output layer

## RNN

For the RNN, each 28 × 28 image was represented as a sequence of:

28 timesteps × 28 features

The RNN processes the image row by row and uses the final timestep representation for digit classification.

# ⚙️ Training

Both models were implemented using PyTorch and trained using:

Cross-Entropy Loss,
Adam Optimizer,
Mini-batch training,
Batch size: 64,
Epochs: 10,

# 📈 Evaluation

Models were evaluated using:

Test Accuracy, 
Confusion Matrix, 
Results, 
Model	Test Accuracy, 
CNN	XX.XX%, 
RNN	XX.XX%

# 🔍 CNN vs RNN

The CNN processes the image as a 2D spatial structure, making it well suited for learning local patterns such as edges, curves, and shapes.

The RNN treats the image as a sequence of rows and learns dependencies across those rows.

This project demonstrates how different neural network architectures can approach the same image-classification problem using different representations of the input data.

# 🛠️ Technologies
Python, 
PyTorch, 
Torchvision, 
NumPy, 
Matplotlib, 
Seaborn, 
Scikit-learn, 
Jupyter Notebook

# 💡 Key Learnings
Image preprocessing and normalization

PyTorch tensors and DataLoaders

CNN architecture and spatial feature extraction

RNN sequence processing

Forward and backward propagation

Model evaluation and confusion matrix analysis

Comparing different deep learning architectures
