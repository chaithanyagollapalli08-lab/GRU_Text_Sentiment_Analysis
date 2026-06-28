# Bidirectional GRU for Text Sentiment Analysis

## Project Overview

This project demonstrates how a **Bidirectional Gated Recurrent Unit (GRU)** neural network can be used for binary sentiment classification on course reviews.

The model analyzes text reviews and classifies them into:

* **Good (Positive)**
* **Bad (Negative)**

It covers the full NLP pipeline including text preprocessing, embedding, sequence modeling, training, and prediction using TensorFlow/Keras.

---

## Dataset

A custom dataset of course feedback reviews was created for training the model.

### Sample Reviews

**Positive Reviews (Label = 1)**

* teacher explained concepts clearly
* course content was excellent
* good learning experience
* assignments were useful
* very informative sessions
* excellent practical examples
* easy to understand topics
* great instructor
* helpful study material
* highly recommended course

**Negative Reviews (Label = 0)**

* teacher explanation was confusing
* course content was poor
* bad learning experience
* assignments were difficult
* boring sessions
* lack of practical examples
* hard to understand topics
* poor instructor
* outdated study material
* not recommended course

---

## Labels

| Label | Sentiment              |
| ----- | ---------------------- |
| **1** | Good (Positive Review) |
| **0** | Bad (Negative Review)  |

---

## Project Workflow

### Step 1: Data Preparation

* Created a custom dataset of course reviews
* Assigned binary sentiment labels
* Split data into training and testing sets

---

### Step 2: Text Preprocessing

* One-Hot Encoding using Keras
* Vocabulary size creation
* Sequence padding using `pad_sequences()`
* Fixed-length input representation

---

### Step 3: Embedding Layer

Words are converted into dense vector representations before being passed into the GRU model.

---

### Step 4: Bidirectional GRU Model

Model Architecture:

* Embedding Layer
* Masking Layer
* Bidirectional GRU Layer
* Bidirectional GRU Layer
* Bidirectional GRU Layer
* Dense Output Layer (Sigmoid Activation)

---

### Step 5: Model Training

* Optimizer: Adam
* Loss Function: Binary Crossentropy
* Evaluation Metric: Accuracy
* Batch Size: 1
* Epochs: Based on training setup

---

### Step 6: Prediction

The trained model predicts whether a given course review is:

* **Good**
* **Bad**

Example:

**Input**

```text
teacher explained concepts clearly
```

**Output**

```text
Good
```

---

## Technologies Used

* Python
* NumPy
* Pandas
* TensorFlow
* Keras
* NLTK

---

## Key Concepts Covered

* Natural Language Processing (NLP)
* Text Preprocessing
* One-Hot Encoding
* Sequence Padding
* Word Embeddings
* Gated Recurrent Unit (GRU)
* Bidirectional GRU
* Binary Sentiment Classification
* Deep Learning

---

## Why GRU?

GRU (Gated Recurrent Unit) is a simplified version of LSTM.

### Advantages of GRU:

* Faster training compared to LSTM
* Fewer parameters
* Efficient for small datasets
* Handles sequence dependencies well

### Bidirectional GRU:

Bidirectional GRU processes text in both forward and backward directions, helping the model understand full context of a sentence.

---

## Future Improvements

* Train on larger real-world datasets
* Apply Dropout for regularization
* Hyperparameter tuning
* Compare with RNN and LSTM models
* Add Attention mechanism or Transformer models
* Deploy using Streamlit or Flask

---

## Learning Outcomes

Through this project, I learned:

* Sequence modeling using GRU
* Difference between RNN, LSTM, and GRU
* Bidirectional neural networks
* Text preprocessing for NLP
* Sentiment classification using deep learning
* Model evaluation using TensorFlow/Keras

---

## Author

**Chaithanya Gollapalli**

Aspiring AI/ML Engineer

Skills: Python | Machine Learning | Deep Learning | NLP | TensorFlow | Keras
