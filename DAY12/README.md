# **Day 12: Building a Simple Neural Network – A Hands-On Tutorial**

Welcome to Day 12 of the **30 Days of Deep Learning** challenge! This repository contains the code, explanations, and outputs for building and training a simple neural network using **TensorFlow** and **PyTorch** for binary classification tasks.

---

## **📋 Overview**
This notebook demonstrates:
1. Loading and preprocessing the **MNIST dataset**.
2. Building and training a simple **neural network** with one hidden layer.
3. Comparing the performance of the model built in TensorFlow and PyTorch.
4. Visualizing training progress with metrics like **accuracy** and **loss**.

---

## **📂 Repository Structure**
```
DAY12/
├── DAY12.ipynb            # Jupyter Notebook with all code and outputs
└── README.md              # This README file
```

---

## **📚 Key Features**
- **Dataset**: MNIST, a dataset of handwritten digits.
- **Task**: Binary classification of digits (0 vs. non-0).
- **Frameworks Used**: TensorFlow and PyTorch.
- **Metrics**: Training accuracy, validation accuracy, and loss plots.

---

## **🛠️ Requirements**
To run the notebook, ensure the following libraries are installed:

### **Python Libraries**
```bash
pip install tensorflow==2.11.0 torch==2.0.1 torchvision matplotlib numpy
```

### **Compatible CUDA and cuDNN Versions**
If you are using a GPU, install the correct versions of CUDA and cuDNN for TensorFlow and PyTorch. Below are the compatibility details:

| Framework      | TensorFlow Version | PyTorch Version | CUDA Version | cuDNN Version | OS           |
|-----------------|--------------------|------------------|--------------|---------------|--------------|
| TensorFlow      | 2.11.0            | -                | 11.2         | 8.1.0         | Windows/Linux/MacOS |
| PyTorch         | -                 | 2.0.1            | 11.7         | 8.5.0         | Windows/Linux/MacOS |

---

## **📖 Usage**
### 1. Clone the Repository
```bash
git clone https://github.com/I-Deepanshu/30-Days-Deep-Learning.git
cd 30-Days-Deep-Learning/DAY12
```

### 2. Run the Notebook
Open the `DAY12.ipynb` file in Jupyter Notebook or Jupyter Lab and execute the cells step-by-step.

```bash
jupyter notebook DAY12.ipynb
```

---

## **📊 Results**
| Framework       | Training Accuracy | Validation Accuracy | Training Time (10 Epochs) |
|------------------|-------------------|----------------------|---------------------------|
| TensorFlow       | 99.1%            | 98.7%               | ~1.2 minutes              |
| PyTorch          | 98.9%            | 98.6%               | ~1.4 minutes              |


---

## **📌 Highlights**
- **Normalization** ensures better convergence of the model.
- TensorFlow provides ease of use with its high-level API, while PyTorch allows flexibility in customization.
- This repository serves as a beginner-friendly guide to neural network implementation.

---

## **🌟 Resources**
- [TensorFlow Documentation](https://www.tensorflow.org/)
- [PyTorch Documentation](https://pytorch.org/)
- [MNIST Dataset](http://yann.lecun.com/exdb/mnist/)

---

## **📅 What's Next?**
Next up in **Day 13**, we’ll explore optimization techniques such as gradient descent, Adam, and other algorithms to train neural networks efficiently.

---

## **📂 GitHub Repository**
Find the full notebook and other resources in the **30 Days of Deep Learning** challenge repository:  
🔗 [GitHub Repository](https://github.com/I-Deepanshu/30-Days-Deep-Learning/tree/main/DAY12)

Feel free to contribute, suggest improvements, or ask questions! 😊
