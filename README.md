# SMS Spam Classification

This project is a **Streamlit web application** that classifies SMS or email messages as either **Spam** or **Not Spam** using a machine learning model.

## Features

- Accepts input text message (SMS or email).
- Preprocesses the text (tokenization, stopword removal, stemming).
- Uses a pre-trained model to predict whether the message is Spam or Not Spam.
- Provides an easy-to-use interface through **Streamlit**.

## How It Works

1. **Preprocessing**: 
   - Converts the text to lowercase.
   - Tokenizes the text.
   - Removes stopwords and punctuation.
   - Stems the remaining words.
   
2. **Vectorization**:
   - Uses **TF-IDF (Term Frequency-Inverse Document Frequency)** vectorization to convert text into numerical format.

3. **Prediction**:
   - The preprocessed and vectorized input is passed to a machine learning model (Logistic Regression or another classifier).
   - The model predicts whether the message is spam or not.

## Installation

To run the project locally, follow these steps:

### Clone the repository:

```bash
git clone https://github.com/your-username/sms-spam-classification.git
cd sms-spam-classification
```

## Install the dependencies:
