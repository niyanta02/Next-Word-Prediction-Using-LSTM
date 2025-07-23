# Next-Word-Prediction-Using-LSTM

LSTM-Based Next Word Generator
Overview
This project implements a next word prediction model using Long Short-Term Memory (LSTM) neural networks. The model is trained on Shakespeare’s Hamlet text dataset to predict the next word given a sequence of words, enabling generation of Shakespearean-style text.

Dataset
Source: Project Gutenberg - Hamlet by William Shakespeare

The text is preprocessed and tokenized to build sequences for training the LSTM model.

Features
Word-level next word prediction using LSTM.

Embedding layer to convert words into dense vectors.

Stacked LSTM layers with Dropout for regularization.

Training with early stopping to prevent overfitting.

Text generation function with temperature sampling to control randomness.

Installation

pip install -r requirements.txt

Prepare the data:
Preprocess the Hamlet text and create input sequences.

Train the model:
Run the training script to train the LSTM model with early stopping.

Generate text:
Use the provided text generation script to generate Shakespearean-style text based on a seed phrase.

python
Copy
Edit
# Example usage:
seed_text = "To be or not to be"
generated_text = generate_text(seed_text, next_words=20, model=model, tokenizer=tokenizer, max_sequence_len=max_sequence_len)
print(generated_text)
Results
Training accuracy improved with more epochs.

Validation loss increased, indicating overfitting.

Future work includes experimenting with GRU models to improve generalization.

License
This project is licensed under the MIT License.
