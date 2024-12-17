# **Computer Vision with Deep Learning: Image Classification, Object Detection, and Image Segmentation**

This repository contains implementations of three essential Computer Vision tasks: **Image Classification**, **Object Detection**, and **Image Segmentation**. Each task is demonstrated using a dedicated Jupyter Notebook and well-documented code to help you learn and implement these techniques in real-world scenarios.

---

## **Repository Structure**

The repository includes the following files and directories:

```
.
├── notebooks/
│   ├── image_classification.ipynb   # Notebook for Image Classification
│   ├── object_detection.ipynb       # Notebook for Object Detection
│   ├── image_segmentation.ipynb     # Notebook for Image Segmentation
├── README.md                        # Repository overview and instructions
├── requirements.txt                 # Python dependencies
└── resources/                       # Additional resources such as saved models, graphs and documentation
```

---

## **Task 1: Image Classification**

### **Overview**
Image classification involves assigning a single label to an input image. The task in this project is performed using the **CIFAR-10 dataset**, which contains 10 classes of images, including airplanes, cars, and animals.

### **Key Features**
- Built with a **Convolutional Neural Network (CNN)** using TensorFlow and Keras.
- Includes data preprocessing, model training, and evaluation.
- Visualizations of training and validation accuracy over epochs.

### **How to Run**
1. Navigate to the `notebooks/` directory.
2. Open `image_classification.ipynb` in Jupyter Notebook or Google Colab.
3. Run the cells to load the CIFAR-10 dataset, train the CNN model, and evaluate its performance.

---

## **Task 2: Object Detection**

### **Overview**
Object detection not only classifies objects in an image but also identifies their locations using bounding boxes. The task uses the **YOLOv5 framework** for detecting objects in images.

### **Key Features**
- Leverages pre-trained YOLOv5 models for real-time object detection.
- Supports detection of multiple objects in an image with bounding boxes and confidence scores.
- Provides examples using the COCO dataset.

### **How to Run**
1. Clone the YOLOv5 repository:
   ```bash
   git clone https://github.com/ultralytics/yolov5.git
   cd yolov5
   pip install -r requirements.txt
   ```
2. Open `object_detection.ipynb` from the `notebooks/` directory.
3. Follow the instructions in the notebook to run object detection on sample images.

---

## **Task 3: Image Segmentation**

### **Overview**
Image segmentation provides pixel-level understanding of an image, classifying each pixel into a predefined category. This project uses a **U-Net architecture** to segment images.

### **Key Features**
- Implements a custom U-Net model for segmentation.
- Includes training, evaluation, and visualization of segmentation results.
- Demonstrates with dummy data for quick experimentation.

### **How to Run**
1. Navigate to the `notebooks/` directory.
2. Open `image_segmentation.ipynb` in Jupyter Notebook or Google Colab.
3. Run the notebook to train the U-Net model on dummy data and visualize segmentation results.

---

## **Setup Instructions**

### **1. Clone the Repository**
```bash
git clone https://github.com/I-Deepanshu/30-Days-Deep-Learning
cd DAY21
```

### **2. Create a Virtual Environment**
```bash
python -m venv cv_env
source cv_env/bin/activate  # On Windows: cv_env\Scripts\activate
```

### **3. Install Dependencies**
```bash
pip install -r requirements.txt
```

### **4. Launch Jupyter Notebook**
```bash
jupyter notebook
```

---

## **Results and Visualizations**

### **Image Classification**
- **Dataset**: CIFAR-10
- **Test Accuracy**: ~72%
- **Graph**: Training vs Validation Accuracy

### **Object Detection**
- **Framework**: YOLOv5
- **Output**: Bounding boxes with labels and confidence scores.

### **Image Segmentation**
- **Model**: U-Net
- **Output**: Pixel-level segmentation of objects in an image.

---

## **Resources**
- **CIFAR-10 Dataset**: [https://www.cs.toronto.edu/~kriz/cifar.html](https://www.cs.toronto.edu/~kriz/cifar.html)
- **YOLOv5 Framework**: [https://github.com/ultralytics/yolov5](https://github.com/ultralytics/yolov5)
- **Pascal VOC Dataset**: [http://host.robots.ox.ac.uk/pascal/VOC/](http://host.robots.ox.ac.uk/pascal/VOC/)

---

## **Upcoming Features**
- Additional datasets for training and testing.
- Hyperparameter tuning examples.
- Streamlit-based UI for testing models.

---

## **Contributing**
Contributions are welcome! If you would like to improve the code or add new features, feel free to open a pull request or raise an issue.

---

## **Author**
This repository is part of a 30-day deep learning journey. For queries or feedback, feel free to connect:    

---

## **License**
This project is licensed under the MIT License. See `LICENSE` for more details.
