# GEN-AI
This is what i learning about GEN AI i will update my weekly learning with practical work


📌 **Text Preprocessing in GenAI**

### 1. Introduction
Before feeding raw text into large language models or training GenAI applications, we must clean and normalize the text. This process is called *text preprocessing*.

In this module, you’ll learn how to:
- Remove noise from raw text
- Normalize the structure (lowercasing, punctuation removal, etc.)
- Tokenize sentences and words
- Remove stopwords
- Perform stemming or lemmatization

Each step is explained with code in the Colab notebook provided.

---
### Dataset https://www.kaggle.com/datasets/lakshmi25npathi/imdb-dataset-of-50k-movie-reviews

### 2. Step-by-Step Breakdown of Notebook

#### ✅ Text Cleaning
- We removed special characters using RegEx:  
  `re.sub(r"[^a-zA-Z0-9]", " ", text)`
- This helps eliminate punctuation and symbols.

#### ✅ Lowercasing
- `text.lower()` converts all characters to lowercase.
- Essential for normalization (e.g., “AI” and “ai” treated the same).

#### ✅ Tokenization
- Using `word_tokenize()` from NLTK to split the text into words.

#### ✅ Stopword Removal
- Stopwords like "is", "the", "and" are removed using `nltk.corpus.stopwords`.

#### ✅ Lemmatization
- Used `WordNetLemmatizer` to reduce words to their base form.
  Example: `studies → study`, `was → be`

---

### 3. Output

The final preprocessed text looks like this:  
`['machine', 'learning', 'model', 'predict', 'price']`

You can now pass this to a vectorizer or GenAI model.

---

### 4. Conclusion

This preprocessing step is a **must** before vectorization, fine-tuning, or inference in any GenAI pipeline.

👉 Use this as a building block for your next NLP or LLM project.

### Next topic is Data representation
