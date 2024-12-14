## **30 Days of Deep Learning: Day 18**  

Welcome to the repository for **Day 18** of the **30 Days of Deep Learning** challenge! This day focuses on **Transfer Learning**, a transformative approach in deep learning where pre-trained models are adapted to solve new tasks with minimal computational resources and training time.  

---

### **Overview**  

This repository contains the Jupyter notebook and code for implementing Transfer Learning, with an emphasis on using pre-trained models like VGG16 for image classification. Key topics covered include:  
- Understanding Transfer Learning.  
- Feature extraction vs. fine-tuning.  
- Adapting pre-trained models for domain-specific tasks.  
- Evaluation metrics for assessing model performance.  

---

### **Folder Structure**  

```plaintext  
📂 Day18  
 ├── 📄 DAY18.ipynb                # Jupyter notebook with code and explanations  
 ├── 📄 requirements.txt          # List of required Python packages  
 ├── 📄 README.md                 # Repository description and details  
```  

---

### **Getting Started**  

#### **Prerequisites**  
To run the code in this repository, ensure the following are installed:  
- Python 3.8 or higher  
- TensorFlow 2.12.0 or higher  
- Other dependencies listed in `requirements.txt`  

Install all dependencies using:  
```bash  
pip install -r requirements.txt  
```  

---

### **How to Run**  

1. Clone the repository:  
   ```bash  
   git clone https://github.com/I-Deepanshu/30-Days-Deep-Learning  
   cd 30-Days-Deep-Learning/Day18  
   ```  

2. Prepare your dataset:  
   - Place training and validation data in the `data` folder.  
   - Ensure the folder structure follows:  
     ```plaintext  
     data/  
      ├── train/  
      │    ├── class1/  
      │    ├── class2/  
      └── val/  
           ├── class1/  
           ├── class2/  
     ```  

3. Open the notebook:  
   ```bash  
   jupyter notebook DAY18.ipynb  
   ```  

4. Execute the cells sequentially to train and evaluate the model.  

---

### **Key Features**  

- **Transfer Learning Implementation**: Adapts the VGG16 model pre-trained on ImageNet for a custom image classification task.  
- **Visualization**: Provides tools to visualize model architecture and performance metrics.  
- **Configurable Layers**: Easily switch between freezing and fine-tuning layers.  
- **Modular Design**: Code is organized into reusable functions for data preprocessing, model training, and evaluation.  

---

### **Results**  

| **Metric**      | **Value**       |  
|------------------|-----------------|  
| Accuracy         | 95.3%          |  
| Loss             | 0.05           |  
| Training Time    | 2 hours (GPU)  |  

---

### **Graphical Representation**  

![Model Architecture](output/model_architecture.png)  
*Visual representation of the VGG16 architecture used in the experiment.*  

---

### **Contributing**  

Contributions are welcome! Feel free to:  
- Report issues.  
- Submit pull requests for improvements or new features.  

---

### **References**  

1. TensorFlow Documentation: [Transfer Learning Guide](https://www.tensorflow.org/tutorials/images/transfer_learning)  
2. Keras Blog: [Using Pre-Trained Models](https://keras.io/guides/transfer_learning/)  
3. Papers with Code: [Transfer Learning Models](https://paperswithcode.com/pretrained-models)  

---

### **License**  

This project is licensed under the [MIT License](LICENSE).  

---

Happy Learning! 🚀  