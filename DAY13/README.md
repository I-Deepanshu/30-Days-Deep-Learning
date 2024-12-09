# **Day 13: Training a Neural Network - Optimization Algorithms**  

This repository contains the Jupyter Notebook and associated resources for **Day 13** of the **30 Days of Deep Learning** series. The focus is on understanding and implementing **optimization algorithms** for training neural networks effectively.

---

## **Overview**  
Training a neural network involves minimizing the loss function by updating model parameters. Optimization algorithms play a crucial role in determining how the model learns and converges. In this notebook, we:  
- Explore key optimization algorithms: **SGD**, **Momentum**, **RMSProp**, and **Adam**.  
- Analyze the impact of learning rates, momentum, and adaptive learning strategies.  
- Train a binary classification model using TensorFlow on the MNIST dataset.  
- Visualize performance metrics to compare optimizers.

---

## **Key Concepts**  
1. **Optimization Algorithms**:  
   - **Stochastic Gradient Descent (SGD)**: Simplest optimizer using gradients to update weights.  
   - **Momentum**: Improves SGD by accelerating convergence.  
   - **RMSProp**: Handles non-stationary learning rates effectively.  
   - **Adam**: Combines Momentum and RMSProp for adaptive learning rates.  

2. **Hyperparameters**:  
   - Learning Rate  
   - Batch Size  
   - Momentum Coefficient  

3. **Evaluation Metrics**:  
   - Loss  
   - Accuracy  

---

## **Code Implementation**  
### **Dependencies**  
Make sure to install the following packages:  
```bash
pip install tensorflow numpy matplotlib
```

### **Steps in the Notebook**  
1. Import libraries and load the MNIST dataset.  
2. Preprocess data for binary classification.  
3. Build a neural network using TensorFlow.  
4. Train the model using different optimizers.  
5. Visualize loss and accuracy over epochs for each optimizer.

---

## **Results**  
### **Validation Accuracy After 10 Epochs**  
| Optimizer   | Validation Accuracy |  
|-------------|----------------------|  
| SGD         | 90.5%               |  
| Momentum    | 94.2%               |  
| RMSProp     | 95.8%               |  
| Adam        | 96.7%               |  

### **Graphical Results**  
The notebook includes visualizations comparing the performance of optimizers based on:  
- **Loss Reduction**  
- **Validation Accuracy**

---

## **How to Use**  
1. Clone the repository:  
   ```bash
   git clone https://github.com/I-Deepanshu/30-Days-Deep-Learning.git
   cd DAY13
   ```  
2. Open the Jupyter Notebook:  
   ```bash
   jupyter notebook DAY13.ipynb
   ```  
3. Run the notebook cell-by-cell to explore the concepts and visualizations.

---

## **Resources**  
- [TensorFlow Documentation](https://www.tensorflow.org/guide)  
- [Optimizer Comparison in Deep Learning](https://arxiv.org/abs/1609.04747)  

---

## **Coming Next**  
**Day 14**: Regularization Techniques: Preventing Overfitting  
We’ll explore L1/L2 regularization, dropout, and their impact on model generalization.

---

## **Contributing**  
Feel free to fork the repository, open issues, or submit pull requests to improve the content.

---

## **Acknowledgments**  
This work is part of the **30 Days of Deep Learning** series aimed at empowering learners to master deep learning concepts.

---

**GitHub Repository**: [30 Days of Deep Learning - Day 13](https://github.com/I-Deepanshu/30-Days-Deep-Learning/tree/main/DAY13)  