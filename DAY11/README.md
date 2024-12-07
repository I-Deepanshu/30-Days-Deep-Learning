# Day 11: Setting Up a Deep Learning Environment  

Welcome to **Day 11** of the **30 Days of Deep Learning** series! In this session, we focus on creating an efficient environment for deep learning using **TensorFlow** and **PyTorch**. This notebook provides a step-by-step guide for configuring GPU support, understanding compatibility between CUDA, cuDNN, and frameworks, and running basic deep learning models.  

---

## 📄 Contents  

- **Overview**  
- **Setup Instructions**  
- **Compatibility Table**  
- **Code Examples**  
- **Performance Comparison**  
- **Resources**  
- **Next Steps**  

---

## 🌟 Overview  

Deep learning frameworks like TensorFlow and PyTorch require optimized environments for high performance. A well-configured GPU environment can drastically reduce training time.  

This notebook covers:  
- Installing and configuring TensorFlow and PyTorch for GPU-based training.  
- CUDA and cuDNN version compatibility for NVIDIA GPUs.  
- Example code for training models on TensorFlow and PyTorch.  
- Performance comparison between the two frameworks.  

---

## 🛠️ Setup Instructions   

### Install Dependencies  

#### For TensorFlow  
```bash  
conda create -n tf_env python=3.9  
conda activate tf_env  
pip install tensorflow  
```  

#### For PyTorch  
```bash  
conda create -n torch_env python=3.9  
conda activate torch_env  
conda install pytorch torchvision torchaudio pytorch-cuda=11.7 -c pytorch -c nvidia  
```  

---

## ⚙️ Compatibility Table  

| Framework       | Version  | CUDA Version | cuDNN Version | Supported GPUs               |  
|------------------|----------|--------------|---------------|-----------------------------|  
| TensorFlow       | 2.12     | 11.8         | 8.6           | NVIDIA Ampere, Pascal, Turing |  
| TensorFlow       | 2.11     | 11.7         | 8.5           | NVIDIA Volta, Turing        |  
| PyTorch          | 2.0      | 11.7         | 8.5           | NVIDIA Ampere, Pascal, Volta |  
| PyTorch          | 1.12     | 11.6         | 8.4           | NVIDIA Turing, Volta        |  

---

## 🧑‍💻 Code Examples  

### TensorFlow Neural Network Example  
```python  
import tensorflow as tf  
from tensorflow.keras import Sequential  
from tensorflow.keras.layers import Dense  

# Define Model  
model = Sequential([  
    Dense(64, activation='relu'),  
    Dense(32, activation='relu'),  
    Dense(1)  
])  

model.compile(optimizer='adam', loss='mse')  
model.fit(tf.random.normal((500, 10)), tf.random.normal((500, 1)), epochs=10)  
```  

### PyTorch Neural Network Example  
```python  
import torch  
import torch.nn as nn  

# Define Model  
class SimpleNN(nn.Module):  
    def __init__(self):  
        super(SimpleNN, self).__init__()  
        self.net = nn.Sequential(  
            nn.Linear(10, 64),  
            nn.ReLU(),  
            nn.Linear(64, 32),  
            nn.ReLU(),  
            nn.Linear(32, 1)  
        )  

    def forward(self, x):  
        return self.net(x)  

model = SimpleNN()  
criterion = nn.MSELoss()  
optimizer = torch.optim.Adam(model.parameters(), lr=0.001)  

# Training  
for epoch in range(10):  
    optimizer.zero_grad()  
    loss = criterion(model(torch.randn(500, 10)), torch.randn(500, 1))  
    loss.backward()  
    optimizer.step()  
```  

---

## 📊 Performance Comparison  

The notebook compares the performance of TensorFlow and PyTorch using:  
1. **Training Time**  
2. **GPU Memory Usage**  

The results are visualized in bar and line graphs for clarity.  

---

## 🔗 Resources  

- [TensorFlow Installation Guide](https://www.tensorflow.org/install)  
- [PyTorch Installation Guide](https://pytorch.org/get-started/locally/)  
- [NVIDIA CUDA Toolkit](https://developer.nvidia.com/cuda-toolkit)  
- [cuDNN Library](https://developer.nvidia.com/cudnn)  
- [Anaconda](https://www.anaconda.com/)  

---

## 📂 Repository Link  

Access the complete notebook on GitHub: [Day 11 Notebook](https://github.com/I-Deepanshu/30-Days-Deep-Learning/blob/main/DAY11/DAY11.ipynb).  

---

## 🚀 Next Steps  

In **Day 12**, we’ll dive into building neural networks from scratch and evaluating their performance.  

✨ Stay tuned and happy coding! ✨  
