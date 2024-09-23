# CS6320 - Natural Language Processing (NLP)  
### Assignment 1: Building an N-Gram Based Language Model

---

## Overview

This project is part of the **CS6320 - Natural Language Processing** course at UT Dallas. The objective is to build and evaluate an n-gram-based language model to predict the next word in a sequence, demonstrating fundamental concepts of statistical language modeling.

## Authors

- **Aankit Das**  
- **Kedar Kadu**  

*Group 21*

---

## Project Goals

The key goals of this project are to:
- Implement a language model using **n-grams** (where n = 1 (unigram) and n = 2 (bigram)).
- Preprocess textual data to ensure the language model functions effectively.
- Explore the effects of different values of `n` in generating text and predicting word sequences.
- Evaluate the model using various metrics, such as perplexity, for assessing language model performance.

## Steps and Workflow

1. **Text Preprocessing:**
   - Tokenization and cleaning of text data (removal of punctuation, stopwords, etc.).
   - Conversion of text to lower case for uniformity.
   
2. **N-Gram Model Construction:**
   - Use bigrams, and trigrams for the language model.
   - Compute n-gram probabilities by calculating the frequency of sequences in the training data.
   
3. **Smoothing Techniques:**
   - Apply smoothing techniques such as **Laplace smoothing**, **Add-k smoothing**, and **Kneser-Ney smoothing** to handle unseen word sequences during testing.

4. **Evaluation:**
   - Test the model on a validation set and compute performance metrics like **perplexity** and **accuracy**.
   - Compare results across different n-gram orders and smoothing techniques.

## Files and Directories

- `A1_DATASET/`  
  Contains the training and testing datasets used for the language model.
  
- `model.ipynb`  
  Python notebook that implements the n-gram model, text preprocessing, and evaluation.

- `README.md`  
  This file, providing an overview of the project.

---

## How to Run

1. **Clone the repository:**
   ```bash
   git clone https://github.com/your-repo/n-gram-language-model.git
   cd n-gram-language-model

2. **Install dependencies:**
   Install necessary Python libraries (e.g., nltk, numpy, etc.) by running:
   ```python
   pip install -r requirements.txt

4. **Run the n-gram model:**
   After installing the necessary packages, we can run the Python notebook 
