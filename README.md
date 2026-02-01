# Twitter Sentiment Analysis using Dictionary-Based Approach

## Problem Description
This project performs **sentiment analysis on Twitter data** using a
**dictionary-based (lexicon-based) approach**.

The objective is to classify tweets as **positive, negative, or neutral**
by leveraging predefined sentiment lexicons rather than supervised machine
learning models. This approach is particularly useful when labeled data is
limited or unavailable.

---

## Dataset
- Source: Twitter data
- Text type: Short, informal social media messages
- Language: English
- Preprocessing required due to noise (URLs, mentions, emojis, hashtags)

---

## Methodology

### Text Preprocessing
- Lowercasing
- Removal of URLs, mentions, hashtags
- Punctuation and stopword removal
- Tokenization

### Sentiment Scoring
- Dictionary-based sentiment lexicon
- Each token contributes a sentiment score
- Tweet-level sentiment is calculated by aggregating token scores

### Sentiment Classification
- Positive sentiment
- Negative sentiment
- Neutral sentiment (score close to zero)

This rule-based method ensures interpretability and transparency in sentiment
decisions.

---

## Evaluation
Since the approach is unsupervised:
- Evaluation is based on sentiment distribution analysis
- Manual inspection of sample tweets
- Comparison of sentiment polarity trends

The focus is on **interpretability rather than predictive accuracy**.

---

## Results
- Tweets are successfully categorized into positive, negative, and neutral classes
- Neutral sentiment dominates, consistent with real-world Twitter data
- The method captures overall sentiment trends effectively

---


---

## Tech Stack
- Python
- pandas
- NumPy
- NLTK
- Matplotlib

---

## How to Run
1. Install dependencies:
pip install -r requirements.txt

2. Run the notebook:
jupyter notebook twitter_sentiment_dictionary_based.ipynb

---

## Key Takeaways
- Demonstrates rule-based NLP and sentiment analysis
- Shows understanding of text preprocessing challenges in social media data
- Provides interpretable sentiment classification without labeled data
- Useful as a baseline before supervised or deep learning approaches

---

## Future Improvements
- Compare with supervised ML models (Logistic Regression, SVM)
- Incorporate emoji and slang sentiment
- Use VADER or other advanced lexicons
- Extend to multilingual sentiment analysis
