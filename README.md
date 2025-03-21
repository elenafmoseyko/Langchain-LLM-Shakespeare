# Hamlet NLP Exploratory Data Analysis

This project explores and analyzes Shakespeare's *Hamlet* using Natural Language Processing (NLP) techniques. 

---

## Dataset

The dataset was sourced from the [TidyTuesday project](https://github.com/rfordatascience/tidytuesday/tree/main/data/2024/2024-09-17) and includes line-by-line dialogue from Shakespeare's *Hamlet*, with columns for:
- `act`
- `scene`
- `character`
- `dialogue`
- `line_number`

---

## Technologies & Libraries

- **Python**
- `pandas`, `numpy` – Data manipulation
- `matplotlib`, `seaborn` – Visualization
- `nltk` – Text cleaning and tokenization
- `wordcloud` – Visual word frequency cloud
- `textblob` – Sentiment analysis
- `gensim` – Topic modeling (LDA)
- `transformers` (Hugging Face) – Summarization & paraphrasing (BART, T5)

---

## Preprocessing Steps

- Removed stopwords and punctuation
- Tokenized text using regex-based tokenizer
- Created a new column `clean_text` for simplified dialogue
- Filtered out empty or non-verbal entries

---

## Exploratory Analysis

- **Word Frequency:** Identified and visualized the most used words
- **Word Cloud:** Illustrated dominant themes visually
- **Top Characters:** Ranked characters by number of spoken lines
- **Sentiment Analysis:** Measured emotional tone of dialogue by character
- **Topic Modeling:** Used LDA to extract thematic clusters from dialogue
- **Text Generation:** Applied BART and T5 for summarization and paraphrasing

---

## Key Insights

- Hamlet is the most active speaker with over 1,400 lines
- Common themes include kingship, revenge, family, and death
- Characters like Reynaldo and Player Queen had the most positive sentiment
- LDA revealed topics aligned with major plot points (e.g., betrayal, confrontation)
- Summarization struggled with Shakespearean style, while T5 handled paraphrasing effectively

---

## Files in this Repo

- `hamlet_nlp_analysis.py` – Main script for data cleaning, visualization, and modeling
- `README.md` – This file



