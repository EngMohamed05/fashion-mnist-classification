# Fashion-MNIST Classification (PyTorch)

This repository contains a PyTorch-based neural network that classifies images from the Fashion-MNIST dataset. The project includes dataset preparation, model training, evaluation, and visualization of predictions.

This is my first machine learning project.

---

## Project Overview

The notebook trains a fully connected neural network on the Fashion-MNIST dataset, which consists of 28x28 grayscale images of clothing items. The model learns to classify images into one of ten categories.

---

## Model Architecture

The implemented model is a simple feed-forward neural network with the following structure:

- Input: 784-dimensional flattened image  
- Hidden Layers:
  - Linear layer + ReLU activation  
  - Linear layer + ReLU activation  
- Output Layer: Linear layer with 10 classes  
- Loss Function: CrossEntropyLoss  
- Optimizer: Adam  
- Metrics: Training accuracy and test accuracy

---

## Training and Evaluation

During training, each epoch logs the following:

```
loss=..., train_acc=..., test_acc=...
```

The notebook also includes:

- Tracking the loss during training  
- Computing accuracy on both training and test sets  
- Displaying a random image from the test set with its true and predicted labels  

---

## How to Run

### 1. Clone the Repository

```bash
git clone https://github.com/EngMohamed05/fashion-mnist-classification.git
cd fashion-mnist-classification
```

### 2. Install Dependencies

Create a `requirements.txt` file with:

```
torch
torchvision
matplotlib
```

Install the dependencies:

```bash
pip install -r requirements.txt
```

### 3. Open the Notebook

```bash
jupyter notebook
```

Then open the `.ipynb` file.

---

## Project Structure

```
.
├── FashionMnist.ipynb
├── dataset/
│   ├── train/
│   └── test/
└── README.md
```

---

## Future Improvements

Possible enhancements include:

- Switching to a convolutional neural network (CNN) for higher accuracy  
- Adding data augmentation  
- Using learning rate scheduling  
- Expanding evaluation with confusion matrices or classification reports  
- Deploying the model using Streamlit or Flask  

---

## Acknowledgments

- Fashion-MNIST dataset by Zalando Research  
- PyTorch documentation  
- matplotlib for visualization  

