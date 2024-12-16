# **Deep Learning for Natural Language Processing (NLP) - Sentiment Analysis**  

This repository contains the implementation of a deep learning model for sentiment analysis on the IMDb dataset. The project uses TensorFlow and Keras to build and train an LSTM-based model to classify movie reviews as either positive or negative.  

---

## **Overview**  

Natural Language Processing (NLP) is a key domain where deep learning techniques have significantly improved the ability of machines to understand and process human language.  
In this project, we implement the following:  
1. Preprocessing the IMDb dataset for training.  
2. Building an LSTM-based architecture to capture the sequential nature of text data.  
3. Visualizing training and validation performance metrics.  

---

## **Project Structure**  

The repository contains the following files:  
- **Day20.ipynb**: Jupyter Notebook with the complete implementation of the project.  
- **requirements.txt**: List of dependencies required to run the project.  
- **README.md**: Discription
---

## **Dataset**  

The dataset used is the **IMDb Reviews Dataset**, a preprocessed dataset of movie reviews, labeled as either positive or negative.  
The dataset is loaded using TensorFlow's `tensorflow.keras.datasets.imdb` module.  

---

## **Model Architecture**  

The model comprises:  
- **Embedding Layer**: Maps words to dense vector representations.  
- **LSTM Layer**: Captures sequential dependencies and context within the text.  
- **Dense Layer**: Outputs binary predictions with a sigmoid activation function.  

---

## **Installation and Setup**  

1. Clone this repository:  
   ```bash
   git clone https://github.com/I-Deepanshu/30-Days-Deep-Learning
   cd DAY20
   ```  

2. Install the required dependencies:  
   ```bash
   pip install -r requirements.txt
   ```  

3. Open the Jupyter Notebook:  
   ```bash
   jupyter notebook Day20.ipynb
   ```  

---

## **Training and Results**  

The model is trained on 25,000 movie reviews (train set) and evaluated on 25,000 reviews (test set).  

### **Key Results:**  

| **Epoch** | **Train Accuracy (%)** | **Validation Accuracy (%)** | **Train Loss** | **Validation Loss** |
|-----------|-------------------------|-----------------------------|----------------|----------------------|
| 1         | 97.30                  | 83.22                       | 0.0822         | 0.5162               |
| 2         | 97.62                  | 82.13                       | 0.0733         | 0.8201               |
| 3         | 98.11                  | 82.88                       | 0.0592         | 0.6727               |
| 4         | 98.68                  | 82.18                       | 0.0421         | 0.6537               |
| 5         | 98.56                  | 82.80                       | 0.0464         | 0.7178               |

---


## **Usage**  

1. **Modify Parameters**:  
   You can adjust hyperparameters like `vocab_size`, `embedding_dim`, `max_length`, etc., in the code to experiment with different configurations.  

2. **Run the Notebook**:  
   Follow the step-by-step implementation in the notebook to preprocess data, train the model, and visualize results.  

3. **Evaluate on Test Data**:  
   After training, evaluate the model to get the final test accuracy.  

---

## **Dependencies**  

The project requires the following Python libraries:  
- `tensorflow`  
- `numpy`  
- `matplotlib`  

Refer to the `requirements.txt` file for the complete list of dependencies.  

---

## **Resources**  

- [Understanding LSTMs](https://colah.github.io/posts/2015-08-Understanding-LSTMs/)  
- [IMDb Dataset](https://ai.stanford.edu/~amaas/data/sentiment/)  
- [TensorFlow Text Classification](https://www.tensorflow.org/tutorials/keras/text_classification)  

---

## **License**  

This project is licensed under the MIT License. See the LICENSE file for details.  

---

## **Author**  

Created by DEEPANSHU.  
Feel free to reach out for any questions or suggestions!  