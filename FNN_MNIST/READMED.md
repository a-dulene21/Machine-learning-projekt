# FNN MNIST Optimization & Weight Initialization

## Project Description

This project focuses on optimizing a simple Feedforward Neural Network (FNN) with one hidden layer for handwritten digit classification using the MNIST dataset.

The main objective is to investigate how different hyperparameters and weight initialization methods affect the model's classification accuracy and training time.

## Objectives

### 1. Hyperparameter Optimization

The following parameters are investigated:

- **Learning Rate:** 0.05, 0.15, 0.25, 0.35, 0.45, 0.55
- **Number of Epochs:** 1, 3, 5, 10, 20
- **Hidden Layer Neurons:** 100, 300, 500, 900, 1200

The goal is to identify the combination that achieves the highest classification accuracy.

### 2. Weight Initialization

Using the best-performing FNN configuration, three different weight initialization methods are compared:

1. **Uniform Distribution:** Weights initialized uniformly between -1 and 1.
2. **Scaled Uniform Distribution:** Weights initialized uniformly between \(-1/\sqrt{n}\) and \(1/\sqrt{n}\), where \(n\) is the number of neurons in the hidden layer.
3. **Normal Distribution:** Weights initialized using a Gaussian distribution with mean 0 and standard deviation 0.5.

The impact of each initialization method on classification accuracy is evaluated.

## Best Current Configuration

| Parameter | Value |
|---|---:|
| Hidden Layer Neurons | 1000 |
| Learning Rate | 0.05 |
| Epochs | 20 |
| Test Accuracy | 98.05% |
| Training Time | 11,921 seconds |
| Testing Time | 7 seconds |

## Dataset

- **Dataset:** MNIST
- **Task:** Handwritten digit classification
- **Input:** 28 × 28 grayscale images
- **Output:** 10 classes (digits 0–9)

## Project Structure

```text
FNN_MNIST/
│
├── README.md
├── datasets/
├
├── FNN_MNIST_Experiment.ipynb

└── requirements.txt
```

## Technologies

- Python
- NumPy
- Matplotlib
- MNIST Dataset
- Feedforward Neural Network (FNN)

## Results

The experimental results will be documented and compared to identify the best hyperparameter configuration and the most effective weight initialization method.

## Author

[Your Name]