Text Summarizer using Hugging Face
Project Overview

This project is a Text Summarization tool built using the Hugging Face Transformers library. It takes a long paragraph as input and generates a concise summary using a pre-trained NLP model.

Features
-Summarizes long text into short, meaningful content
-Uses pre-trained state-of-the-art models
-Simple and easy to use
-Compatible with Google Colab and Jupyter Notebook

Technologies Used
-Python
-Transformers (Hugging Face)
-PyTorch

Project Workflow
-Data Input: User provides a long paragraph
-Model Loading: Pre-trained summarization model is loaded
-Processing: Text is analyzed and summarized
-Output: A short summary is generated

Installation
Install the required libraries:
-pip install transformers
-pip install torch
Usage
from transformers import pipeline
# Load summarization pipeline
summarizer = pipeline("summarization", model="facebook/bart-large-cnn")

# Input text
text = """Your long paragraph here"""

# Generate summary
summary = summarizer(text, max_length=60, min_length=20, do_sample=False)

print(summary[0]['summary_text'])

pipeline("summarization", model="facebook/bart-large-cnn")

Slow performance
Suggestion: Use GPU in Google Colab

Future Improvements
-Add a graphical user interface
- as a web application
-Add multilingual support
-Allow dynamic summary length

Author
Suryakanta Baut
