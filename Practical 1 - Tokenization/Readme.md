# Text Preprocessing using NLTK

This file contains the code for NLP Practical 1. The goal of this notebook is to implement fundamental text preprocessing techniques using Python's Natural Language Toolkit (`nltk`).

## Project Overview

The notebook demonstrates the following text processing steps on a sample text:

- **Tokenization:** Breaking down a string into individual tokens. The code compares five different methods to show how they handle punctuation, hashtags, and specific phrases:
  1. `WhitespaceTokenizer`
  2. `WordPunctTokenizer`
  3. `TreebankWordTokenizer`
  4. `TweetTokenizer` 
  5. `MWETokenizer` 

- **Stemming:** Reducing words to their root form by stripping suffixes (e.g., converting "learning" to "learn"). 
  - Implemented using `PorterStemmer` and `SnowballStemmer`.

- **Lemmatization:** Converting words to their meaningful base dictionary form based on their context.
  - Implemented using `WordNetLemmatizer`.

## Setup Instructions

1. Install the required library:
   ```bash
   pip install nltk
   ```
2. Open `NLP 1st.ipynb` in Jupyter Notebook, VS Code, or Google Colab.
3. Run the cells sequentially. The necessary NLTK datasets (`wordnet` and `omw-1.4`) will download automatically during the first run.
