# NLP Practical 3: Text Cleaning and Preprocessing

## Problem Statement
Perform text cleaning, perform lemmatization, remove stop words, and apply label encoding. Create representations using TF-IDF. Save outputs. The dataset to be used is `News_dataset.pickle`.

## Explanation
This practical demonstrates the standard pipeline for preparing raw text data for machine learning models.
1. **Data Loading:** The `.pickle` dataset was loaded using pandas. A subset of 100 rows was used to ensure fast execution.
2. **Text Cleaning:** A custom function was built to process the 'Content' column. It converts text to lowercase, removes special characters using regular expressions, removes English stopwords, and applies WordNet Lemmatization to extract the root form of words.
3. **Label Encoding:** The target 'Category' column was transformed from text into numerical integer labels using scikit-learn's `LabelEncoder`.
4. **TF-IDF Vectorization:** The cleaned text was converted into numerical features using `TfidfVectorizer`, resulting in a matrix shape of `(100, 4514)`.
5. **Saving Outputs:** The final TF-IDF feature matrix and the encoded target labels were serialized and saved to the local disk as `.pkl` files using the `pickle` library.

## Conclusion
Data preprocessing is an essential step in NLP. By successfully applying text cleaning, lemmatization, and TF-IDF vectorization, we transformed unstructured, noisy news text into a structured, numerical format. The saved output files are now fully ready to be fed into any machine learning classification algorithm.
