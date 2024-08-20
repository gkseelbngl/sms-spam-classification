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

```bash
pip install -r requirements.txt
```

## Run the application:

```bash
streamlit run app.py
```

## Files

- **app.py:** The main Python file containing the Streamlit application.
- **model.pkl:** The pre-trained machine learning model for predicting spam messages.
- **vectorizer.pkl:** The TF-IDF vectorizer used to preprocess text.
- **requirements.txt:** The file that lists all the dependencies required to run the project.

## Usage

1. After running the application, a web interface will open in your browser.
2. Enter the message you want to classify in the text box.
3. Click the **Predict** button.
4. The model will classify the message as either **Spam** or **Not Spam**.

## Example

```bash
Enter the message: "Congratulations! You've won a $1000 gift card. Call now!"
Prediction: Spam
```

## Dependencies

The following Python libraries are required:

- Streamlit
- NLTK
- Scikit-learn
- Pickle

Install these using the **`requirements.txt`** file:
```bash
pip install -r requirements.txt
```

## Acknowledgments

This project uses the following tools:

- Streamlit for building the interactive web application.
- Scikit-learn for training and using machine learning models.
- NLTK for natural language processing tasks like tokenization and stopword removal.
