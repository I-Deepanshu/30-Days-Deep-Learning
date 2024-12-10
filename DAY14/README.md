# **Day 14: Regularization Techniques – Preventing Overfitting in Neural Networks**

Welcome to **Day 14** of the **30 Days of Deep Learning** series! This repository focuses on regularization techniques used to improve the generalization capability of neural networks and reduce overfitting.

---

## **Overview**
Overfitting occurs when a model performs well on training data but poorly on unseen data. Regularization introduces constraints to the model to reduce its complexity and enhance its ability to generalize. This repository demonstrates several regularization techniques such as L1/L2 regularization, dropout, early stopping, and more.

---

## **Techniques Covered**
### 1. **L1 and L2 Regularization**
- Adds penalties to the loss function based on weights.
- Helps reduce the model's complexity.

### 2. **Dropout**
- Randomly deactivates neurons during training.
- Prevents over-reliance on specific neurons.

### 3. **Early Stopping**
- Halts training when validation performance stops improving.

### 4. **Batch Normalization**
- Stabilizes learning by normalizing intermediate layers.

### 5. **Data Augmentation**
- Expands training data by applying transformations.

### 6. **Simplified Models**
- Reduces the number of parameters to avoid overfitting.

---

## **Dataset**
This repository uses the **MNIST dataset**, which contains grayscale images of handwritten digits (0-9). Each image is of size 28x28 pixels.

---

## **Code Implementation**
The implementation is done using TensorFlow, covering models:
1. Without regularization.
2. With L2 regularization.
3. With dropout layers.

---

## **Results**
### **Validation Accuracy Comparison**
| Regularization Technique | Validation Accuracy (Epoch 10) |
|--------------------------|---------------------------------|
| No Regularization        | 94.8%                          |
| L2 Regularization        | 96.1%                          |
| Dropout                  | 95.4%                          |

### **Graphs**
Validation accuracy graphs for different techniques are plotted to compare their effectiveness.

---

## **How to Run the Code**
1. Clone the repository:
   ```bash
   git clone https://github.com/I-Deepanshu/30-Days-Deep-Learning.git
   cd DAY14
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Run the Jupyter Notebook:
   ```bash
   jupyter notebook DAY14.ipynb
   ```

---

## **Key Files**
- **`DAY14.ipynb`**: Jupyter Notebook with code, outputs, and visualizations.
- **`requirements.txt`**: List of Python dependencies.

---

## **Resources**
- [Deep Learning Book](https://www.deeplearningbook.org/)
- [TensorFlow Regularization Guide](https://www.tensorflow.org/tutorials)
- [Andrew Ng’s Machine Learning Course](https://www.coursera.org/learn/machine-learning)

---

## **Coming Next**
**Day 15: Hyperparameter Tuning**  
In the next session, we will explore how to find the best configuration for your models using hyperparameter tuning.

---

## **GitHub Repository**
The complete notebook and implementation are available on GitHub:  
[**Day 14: Regularization Techniques**](https://github.com/I-Deepanshu/30-Days-Deep-Learning/tree/main/DAY14)

---

Let’s keep learning and building towards mastering deep learning! 🚀