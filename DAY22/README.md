# **Translator Model for Machine Translation**  

This repository contains the implementation of a Seq2Seq Translator model for machine translation using TensorFlow and TensorFlow Datasets. The model is trained to translate Portuguese (pt) sentences to English (en) using the TED Talks dataset provided by TensorFlow Datasets (`ted_hrlr_translate/pt_to_en`).  

---

## **Features**  

- **Seq2Seq Model**: Built using an `Embedding` layer, an `LSTM` layer, and a `Dense` layer.  
- **Custom Tokenization**: Implements subword tokenization for efficient text encoding.  
- **Dynamic Padding**: Prepares data with padding to accommodate variable-length sequences.  
- **Validation Pipeline**: Includes training and validation datasets for performance evaluation.  

---

## **Requirements**  

To run this project, install the required dependencies using:  

```bash  
pip install -r requirements.txt  
```  

### **Dependencies**  
- `tensorflow==2.11.0`  
- `tensorflow-datasets==4.10.0`  

---

## **Dataset**  

We use the **TED Talks Translation Dataset**:  
- **Dataset Name**: `ted_hrlr_translate/pt_to_en`  
- **Description**: A dataset containing Portuguese-English sentence pairs for translation tasks.  
- **Download and Prepare**: The dataset is automatically downloaded and prepared using TensorFlow Datasets.  

---

## **Model Architecture**  

The model consists of the following layers:  

1. **Embedding Layer**: Converts input tokens into dense vectors.  
2. **LSTM Layer**: Processes sequences to capture context for translation.  
3. **Dense Layer**: Produces predictions over the target vocabulary.  

### **Model Summary**  
| Layer          | Output Shape      | Trainable Params |  
|-----------------|-------------------|------------------|  
| Embedding       | (None, None, 64)  | `vocab_size * 64` |  
| LSTM            | (None, None, 128) | `(128 * (64 + 128 + 1))` |  
| Dense           | (None, None, vocab_size) | `128 * vocab_size` |  

---

## **Training and Evaluation**  

### **Training**  

The model is trained using the following configuration:  
- **Loss Function**: `sparse_categorical_crossentropy`  
- **Optimizer**: Adam  
- **Batch Size**: 64  
- **Epochs**: 3  

### **Results**  
The model achieves reasonable accuracy on both training and validation datasets within three epochs.  

---

## **Usage**  

### **Training the Model**  
Run the `translator_training.py` script to train the model:  

```bash  
python translator_training.py  
```  

### **Test the Model**  
Provide input sentences in Portuguese to test translations into English:  

```python  
input_sentence = "Olá, como vai você?"  
translated_sentence = translator.predict(input_sentence)  
print(f"Translation: {translated_sentence}")  
```  

---

## **Code Walkthrough**  

### **Tokenization**  
The tokenizer is built using `SubwordTextEncoder`:  
```python  
tokenizer_en = tfds.deprecated.text.SubwordTextEncoder.build_from_corpus(...)  
tokenizer_pt = tfds.deprecated.text.SubwordTextEncoder.build_from_corpus(...)  
```  

### **Data Preparation**  
The data is processed into padded sequences with start and end tokens for both input and target sequences.  

### **Model Implementation**  
The Seq2Seq model uses an embedding layer followed by an LSTM decoder:  
```python  
class Translator(tf.keras.Model):  
    def __init__(self, vocab_size, embedding_dim, units):  
        super().__init__()  
        self.embedding = Embedding(vocab_size, embedding_dim)  
        self.lstm = LSTM(units, return_sequences=True, return_state=True)  
        self.fc = Dense(vocab_size)  
```  

---

## **Graph and Results**  

### **Loss and Accuracy Trends**  

| Epoch | Training Loss | Validation Loss | Training Accuracy | Validation Accuracy |  
|-------|---------------|-----------------|-------------------|---------------------|  
| 1     | 0.0822        | 0.5162          | 0.9730            | 0.8322              |  
| 2     | 0.0733        | 0.8201          | 0.9762            | 0.8213              |  
| 3     | 0.0592        | 0.6727          | 0.9811            | 0.8288              |  

---

## **Resources**  

- **Dataset**: [TensorFlow Datasets](https://www.tensorflow.org/datasets/catalog/ted_hrlr_translate)  
- **TensorFlow Documentation**: [Keras API](https://www.tensorflow.org/guide/keras)  

---

## **GitHub Repository**  

The complete code and resources for this project are available in the GitHub repository:  
[GitHub Repo](https://github.com/I-Deepanshu/30-Days-Deep-Learning/tree/main/DAY22)  

--- 

Feel free to raise issues or contribute by submitting pull requests!