# IMDB Movie Review Sentiment Analysis using Simple RNN

## Overview

This project is a Deep Learning-based sentiment analysis application that classifies IMDB movie reviews as **Positive** or **Negative**. The model is built using a **Simple Recurrent Neural Network (Simple RNN)** with TensorFlow/Keras and deployed using Streamlit for an interactive web interface.

Users can enter any movie review, and the application predicts its sentiment along with a prediction score.

---

## Features

* Binary sentiment classification (Positive/Negative)
* Interactive Streamlit web application
* Real-time sentiment prediction
* Pre-trained Simple RNN model
* Text preprocessing using the IMDB word index
* Displays prediction confidence score

---

## Tech Stack

* Python
* TensorFlow
* Keras
* NumPy
* Streamlit

---

## Project Structure

```text
IMDB-Sentiment-Analysis/
│
├── app.py                     # Streamlit application
├── simple_rnn_imdb.h5         # Trained model
├── requirements.txt           # Project dependencies
├── README.md                  # Project documentation
└── notebooks/
    └── model_training.ipynb   # Model training notebook (optional)
```

---

## Model Architecture

* Embedding Layer
* Simple RNN Layer
* Dense Output Layer (Sigmoid Activation)

**Loss Function:** Binary Crossentropy

**Optimizer:** Adam

**Evaluation Metric:** Accuracy

---

## Dataset

This project uses the IMDB Movie Reviews Dataset provided by TensorFlow/Keras.

* 50,000 movie reviews
* Binary sentiment classification
* 25,000 training samples
* 25,000 testing samples
* Vocabulary limited to the top 10,000 most frequent words

---

## Installation

### Clone the repository

```bash
git clone https://github.com/your-username/imdb-sentiment-analysis.git
```

### Navigate to the project directory

```bash
cd imdb-sentiment-analysis
```

### Create a virtual environment (Optional)

**Windows**

```bash
python -m venv venv
venv\Scripts\activate
```

**Linux/macOS**

```bash
python3 -m venv venv
source venv/bin/activate
```

### Install dependencies

```bash
pip install -r requirements.txt
```

---

## Run the Application

```bash
streamlit run app.py
```

Then open:

```text
http://localhost:8501
```

---

## How It Works

1. User enters a movie review.
2. The review is converted to lowercase.
3. Words are mapped to their corresponding IMDB indices.
4. The sequence is padded to a fixed length.
5. The trained Simple RNN model predicts the sentiment.
6. The application displays:

   * Predicted sentiment
   * Prediction score

---

## Example

### Input

```text
This movie was absolutely amazing. The acting and storyline were fantastic.
```

### Output

```text
Sentiment: Positive
Prediction Score: 0.9876
```

---

## Requirements

```text
streamlit
tensorflow==2.15.0
numpy
```

---

## Future Improvements

* Replace Simple RNN with LSTM or GRU
* Improve preprocessing using a custom tokenizer
* Add confidence visualization
* Support batch predictions
* Deploy on Streamlit Community Cloud

---

## Author

**Sahil Patil**

Third-Year Engineering Student, VIT Pune

**Areas of Interest**

* Artificial Intelligence
* Machine Learning
* Deep Learning
* Natural Language Processing
* TensorFlow
* Python
