# TextSummarizer-FineTuned-BART

This repository contains a fine-tuned **BART** model for text summarization using the Hugging Face Transformers library.  
It trains the model on a custom dataset and evaluates its performance using ROUGE metrics.

---

## Overview
The project fine-tunes a pre-trained summarization model using CSV datasets (train, validation, test).  
It includes a cleaning function to handle corrupted lines, encoding issues, and missing columns before training.

Main steps:
- Dataset cleaning and preprocessing  
- Model fine-tuning  
- Evaluation and inference testing  

---

## Features
- Handles malformed CSV files  
- Fine-tunes `facebook/bart-large-cnn` or similar models  
- Evaluation with ROUGE scores  
- Interactive summarization testing  


---

## Model
Uses **BART** (Bidirectional and Auto-Regressive Transformers), an encoder-decoder model designed for abstractive summarization.  
Alternative models can be used, such as:
- `t5-small`
- `t5-base`
- `google/pegasus-xsum`

---

## Requirements
Install dependencies:
```bash
pip install -r requirements.txt

transformers
datasets
evaluate
torch
pandas
numpy
tqdm
