# Practical Implementation of TF-IDF / Text Preprocessing in Python

This notebook demonstrates a basic NLP text-processing workflow using NLTK and scikit-learn. Despite the project name, the current notebook focuses on text cleaning, tokenization, stemming, lemmatization, stopword removal, and bag-of-words vectorization with `CountVectorizer`.

## What the notebook does

- Loads a sample paragraph about Khan Abdul Ghaffar Khan
- Splits the paragraph into sentences
- Downloads the required NLTK resources
- Applies tokenization, stopword removal, and normalization
- Demonstrates stemming with `PorterStemmer`
- Demonstrates lemmatization with `WordNetLemmatizer`
- Builds a bag-of-words representation using `CountVectorizer`
- Shows the resulting vocabulary and vector output for the first sentence

## Requirements

- Python 3.9 or later
- Jupyter Notebook or VS Code Notebook support
- Packages:
  - `nltk`
  - `scikit-learn`
  - `numpy` and `scipy` as dependencies of scikit-learn

## Install dependencies

If you are running this notebook in a fresh environment, install the packages with:

```bash
pip install nltk scikit-learn
```

## NLTK resources used

The notebook downloads these corpora/models at runtime:

- `punkt`
- `punkt_tab`
- `stopwords`
- `wordnet`
- `omw-1.4`

If downloads fail because of network restrictions, install them manually in an environment with internet access.

## How to run

1. Open `main.ipynb` in Jupyter or VS Code.
2. Run the cells from top to bottom.
3. Review the printed sentences, cleaned corpus, stemming output, lemmatization output, and bag-of-words matrix.

## Output summary

The notebook produces:

- A list of tokenized sentences
- A cleaned text corpus
- Stemmed and lemmatized word examples
- A learned vocabulary from `CountVectorizer`
- A sparse bag-of-words matrix for the corpus

## Notes

- The notebook currently implements bag-of-words rather than TF-IDF.
- If you want an actual TF-IDF version, replace `CountVectorizer` with `TfidfVectorizer` and fit it on the cleaned corpus.

## Project Structure

- `main.ipynb` - notebook containing the full preprocessing and vectorization example
