Hamlet NLP + LLM Paraphrasing Analysis
This project explores how large language models (LLMs) interpret and rephrase Shakespeare's Hamlet using LangChain, Ollama, and classic NLP techniques.
We paraphrase the original lines into natural modern English, then run sentiment analysis, topic modeling, and lexical comparisons between the original and AI-generated versions.

Dataset
The original dataset comes from the TidyTuesday project, featuring line-by-line Hamlet dialogue, including:

act

scene

character

dialogue

line_number

The file hamlet_paraphrased.csv contains an additional paraphrased column with AI-rewritten lines.

Pipeline Overview
🔹 Input: Shakespearean dialogue from hamlet.csv
🔹 LangChain PromptTemplate: Formats the prompt
🔹 Ollama: Runs a local LLM (e.g., mistral, phi)
🔹 Output: Paraphrased modern English
🔹 Analysis: NLP tools used for comparison

Diagram available in repo: langchain_pipeline_diagram.png

Technologies & Libraries
LangChain + Ollama – Prompt orchestration + local LLM inference

Python – Core programming language

pandas, numpy – Data manipulation

matplotlib, seaborn – Visualization

nltk, textblob – Text cleaning, sentiment analysis

wordcloud – Word frequency visualizations

gensim, bertopic – Topic modeling (LDA + transformer-based)

transformers (T5, BART) – Baseline summarization and paraphrasing

NLP & LLM Analysis
Paraphrasing with LangChain + Ollama LLMs (offline)

Sentiment Analysis comparing original vs paraphrased (TextBlob)

Topic Modeling with both LDA and BERTopic

Lexical Complexity: Sentence length, word frequency, simplification

Per-Character Emotion Profiling

Side-by-Side Comparisons of lines pre- and post-paraphrasing

Key Insights
Tone Shifts: The AI reworded emotionally intense lines with milder language.

Topic Drift: Key themes (e.g. betrayal, kingship) remained, but some nuance was lost.

Character Rebalancing: Supporting characters lost verbal richness in paraphrasing.

Performance: Local models via Ollama were fast, private, and surprisingly accurate.

Files in This Repo
hamlet.csv – Original dataset

hamlet_paraphrased.csv – With AI-generated modern English lines

topics_labeled.csv – Topic modeling output with human-readable labels

shakespeare_paraphrasing_with_langchain.ipynb – End-to-end LangChain + NLP pipeline

langchain_pipeline_diagram.png – Visual flow of LLM pipeline

README.md – This file




