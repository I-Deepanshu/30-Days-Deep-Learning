# Day 15: Hyperparameter Tuning – Unlocking the Full Potential of Deep Learning Models

This repository contains all resources, code, and visualizations for **Day 15** of the **30 Days of Deep Learning** series. The focus is on understanding and applying hyperparameter tuning techniques to optimize deep learning models.

## 📋 Overview

Hyperparameter tuning is a critical step in machine learning and deep learning. It involves finding the best set of hyperparameters for a model to maximize its performance on a validation dataset. This project explores:
- Key hyperparameters for deep learning models (e.g., learning rate, batch size, optimizer, etc.).
- Techniques like grid search, random search, and Bayesian optimization.
- Visualization of the impact of hyperparameters on model performance.
- Implementation of a neural network with hyperparameter tuning.

---

## 🛠️ Code Details

### 1. **Data Preparation**
- Dataset: **MNIST** dataset of handwritten digits.
- Train and test splits prepared using TensorFlow/Keras.

### 2. **Model Design**
- A fully connected neural network (Multilayer Perceptron).
- Key features:
  - Varying dropout rates.
  - Different learning rates.
  - Multiple optimizers (SGD, Adam).

### 3. **Hyperparameter Tuning**
- Techniques:
  - **Grid Search**: Exhaustively explores all hyperparameter combinations.
  - **Random Search**: Samples hyperparameter combinations randomly.
- Metrics: Validation accuracy and loss.

### 4. **Visualization**
- Heatmap of validation accuracy across different combinations of learning rates and dropout rates.
- Line plots showing the training and validation curves.

---

## 📊 Results

### Best Hyperparameters:
| **Hyperparameter** | **Optimal Value** |
|---------------------|-------------------|
| Learning Rate       | 0.001             |
| Dropout Rate        | 0.2               |
| Optimizer           | Adam              |

### Accuracy:
- Best Validation Accuracy: **86.5%**

### Visualization:
![Heatmap of Validation Accuracy](path_to_heatmap.png)

---

## 🔧 Installation and Usage

### Prerequisites:
- Python 3.8+
- TensorFlow 2.10+
- Matplotlib
- NumPy

### Steps to Run:
1. Clone the repository:
   ```bash
   git clone https://github.com/I-Deepanshu/30-Days-Deep-Learning/tree/main/DAY15
   ```
2. Install required libraries:
   ```bash
   pip install -r requirements.txt
   ```
3. Run the Jupyter Notebook:
   ```bash
   jupyter notebook DAY15.ipynb
   ```

---

## 📈 Graphical Representation Code

The repository also includes code for creating a heatmap to visualize the validation accuracy for different hyperparameter combinations.

---

## 🔗 Resources

- **TensorFlow Documentation**: [TensorFlow](https://www.tensorflow.org)
- **MNIST Dataset**: [MNIST Handwritten Digits](http://yann.lecun.com/exdb/mnist/)
- **Hyperparameter Tuning with Keras**: [Keras Tuning Guide](https://keras.io/guides/keras_tuner/)

---

## 🌟 What's Next?

The next session (Day 16) focuses on **Generative Adversarial Networks (GANs)**, where we explore how to generate synthetic data using adversarial learning techniques.

---

## 📂 Repository Structure
```plaintext
DAY15/
├── DAY15.ipynb               # Jupyter Notebook with all code
├── README.md                 # This file
├── requirements.txt          # Dependencies for the project
├── heatmap.png               # Heatmap visualization
└── outputs/                  # Directory for saved results and outputs
```

---

## 📬 Contact

If you have any questions or feedback, feel free to reach out:
- LinkedIn: [Your LinkedIn Profile](https://www.linkedin.com/in/deepanshu-shimar-704633256/)
- GitHub: [Your GitHub Profile](https://github.com/I-Deepanshu)

---

This repository is part of the **30 Days of Deep Learning** series, aiming to provide hands-on experience with deep learning concepts.

