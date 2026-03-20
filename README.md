Overview

This project is a Text Summarization tool built using Hugging Face Transformers. It takes long text input and generates a concise summary using a pre-trained model.

Features

Uses facebook/bart-large-cnn model

Custom tokenizer and model loading

Handles long text (up to 1024 tokens)

Interactive input system

Displays word reduction

Tech Stack

Python

Hugging Face Transformers

PyTorch

Installation
pip install transformers torch accelerate
Usage

Run the notebook and enter text when prompted:

summarizer = initialize_summarizer()
print(summarize_text(summarizer, "Your long text here"))
Example

Input: Long paragraph
Output: Short meaningful summary

Author

Suryakanta Baut
