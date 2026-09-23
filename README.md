# SentimentScope - IMDB Sentiment Analysis with Transformers

SentimentScope is a sentiment analysis project developed as part of the **Udacity AI Programming program**.

The goal of the project is to build and train a transformer-based model capable of classifying IMDB movie reviews as either **positive** or **negative**.

The project covers the complete machine learning workflow, from dataset preparation and tokenization to model training, validation, and evaluation.

## Project Objectives

The main objectives of this project are to:

- Load and explore the IMDB movie review dataset
- Analyze sentiment distribution and review lengths
- Prepare training, validation, and test datasets
- Tokenize movie reviews using the `bert-base-uncased` tokenizer
- Implement a custom PyTorch `Dataset`
- Create PyTorch `DataLoader` objects for batch processing
- Adapt a transformer architecture for binary classification
- Implement the model training and validation loops
- Evaluate the trained model on unseen test data
- Save the trained model checkpoint for later inference

## Dataset

The project uses the **IMDB Large Movie Review Dataset**, which contains labeled movie reviews for binary sentiment classification.

Each review is classified as:

- `0` - Negative
- `1` - Positive

## Model & Training

The project uses a custom transformer-based model for binary sentiment classification.

Reviews are tokenized with `bert-base-uncased`, padded or truncated to a maximum sequence length of 128 tokens, and processed in batches using PyTorch `DataLoader`.

The model was trained with:

- Cross-entropy loss
- AdamW optimizer
- Learning rate: `3e-4`
- Batch size: `32`
- 5 training epochs

## Results

Validation accuracy improved throughout training, reaching **79.36%** after 5 epochs.

The final model achieved a test accuracy of **76.62%**, exceeding the project requirement of 75%.

## Acknowledgements

This project was completed as part of the **Udacity AI Programming program**.