# PDF Text Summarizer

A Python-based tool that uses the BART (Facebook/bart-large-cnn) transformer model to generate concise summaries from PDF documents.

## Features

- Upload PDF documents
- Adjustable summary length controls
- Download summarized content as PDF
- Handles large documents by chunking text
- Browser-based interface using Jupyter widgets

## Try it Online

You can try this notebook directly in Google Colab:
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1O-8r695Xedj89AaAy87lNWLyTZA8NeSz?usp=sharing)

## Requirements

- Python 3.6+
- transformers
- PyPDF2
- torch
- tqdm
- ipywidgets
- fpdf2

## Usage

1. Upload a PDF file using the "Upload PDF" button
2. Adjust the summary length parameters using the sliders:
   - Max Length: Controls the maximum length of the summary
   - Min Length: Controls the minimum length of the summary
3. Once processing is complete, click "Download Summary" to get your summarized PDF

## Local Setup

1. Clone this repository
2. Install requirements:
```bash
pip install transformers PyPDF2 torch tqdm ipywidgets fpdf2
```
3. Open the notebook in Jupyter or VS Code with Jupyter extension
4. Run all cells

## Note

The summarization process may take some time depending on:
- The size of your PDF document
- Your hardware capabilities
- Whether you're using GPU or CPU for processing