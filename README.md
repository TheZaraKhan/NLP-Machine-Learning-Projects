# NLP & Machine Learning Projects

This repository contains a collection of my research experiments and Python projects in **Natural Language Processing (NLP), neural networks, and machine learning**.

The projects include my master's research on automatic paraphrase generation for Urdu, multilingual language identification, and text classification. They demonstrate my experience in dataset preparation, neural model development, feature engineering, and experimental evaluation.

The original notebooks have been preserved to document my research and development work.

---

## 1. [Automatic Paraphrase Generation for Urdu](01-Urdu-Paraphrase-Generation/)

**Master's Research | Neural NLP | Sequence-to-Sequence Learning**

This project is part of my master's thesis, *Automatic Paraphrase Generation for the Urdu Language*, which investigated neural approaches to generating paraphrases for Urdu.

The repository includes selected experiments on **lexical paraphrase generation**, covering three stages:

- **Data Preparation:** Processing and preparing Urdu lexical paraphrase pairs for model training.
- **Neural Model Training:** Implementing and training an encoder-decoder Seq2Seq architecture using LSTM networks and word embeddings.
- **Model Evaluation:** Evaluating generated paraphrases using BLEU and ROUGE metrics.

The included notebooks represent one component of my broader research involving four Urdu paraphrase datasets.

**Technologies:** Python, TensorFlow, Keras, LSTM, Seq2Seq, NLP, BLEU, ROUGE.

**Research Publication:**

*Automatic Paraphrase Generation at Phrasal, and Sentence Level for Urdu Language: Data and Methods* — SAGE Journals, 2025.

---

## 2. [Language Identification using Machine Learning](02-Language-Identification/)

**Multilingual NLP | Text Classification | Machine Learning**

This project explores automatic language identification using supervised machine learning and different text feature representations.

**Key components:**

- Curated a multilingual dataset containing 22 languages by extracting data from an existing collection of CSV files and modifying language labels.
- Implemented word-level and character-level n-gram feature extraction.
- Trained and compared Random Forest, Linear SVC, and Logistic Regression classifiers.
- Evaluated classification accuracy across different feature configurations.

The experiments use 22,000 text samples to investigate the effectiveness of different machine learning approaches to language identification.

**Technologies:** Python, Scikit-learn, Pandas, NumPy, CountVectorizer.

**Original Kaggle Resources:**
- [Machine Learning Notebook](https://www.kaggle.com/code/zarajamshaid/language-identification-machine-learning)
- [Language Identification Dataset](https://www.kaggle.com/datasets/zarajamshaid/language-identification-datasst)

---

## 3. [Basic NLP on Disaster Tweets](03-Disaster-Tweet-Classification/)

**Text Preprocessing | Feature Engineering | Classification**

An exploratory NLP project focused on processing and classifying social media text related to disasters.

**Techniques covered:**

- Text cleaning, tokenization, and stopword removal
- Word frequency analysis and n-gram extraction
- CountVectorizer and TF-IDF representations
- Logistic Regression classification
- Model evaluation and feature selection

This notebook was adapted from the original work by [Holf Yuen](https://www.kaggle.com/code/holfyuen/basic-nlp-on-disaster-tweets) and is included as part of my earlier NLP learning and experimentation.

**Technologies:** Python, Scikit-learn, Pandas, NLP, TF-IDF.

**Original Kaggle Notebook:** [Basic NLP on Disaster Tweets](https://www.kaggle.com/code/zarajamshaid/basic-nlp-on-disaster-tweets)

---

## Technical Skills Demonstrated

| Area | Tools & Techniques |
|---|---|
| Programming | Python |
| Deep Learning | TensorFlow, Keras, LSTM, Seq2Seq |
| Machine Learning | Scikit-learn, Random Forest, Linear SVC, Logistic Regression |
| NLP | Text preprocessing, tokenization, n-grams, text classification, paraphrase generation |
| Data Processing | Pandas, NumPy |
| Evaluation | BLEU, ROUGE, accuracy, F1-score |
| Development | Jupyter Notebook, Google Colab, Kaggle |

---

## About This Repository

These projects document my earlier academic research and practical work in NLP and machine learning. The notebooks are retained in their original form, including their experimental code and available outputs.

Some notebooks depend on historical datasets, external files, or earlier library versions and may require additional setup to reproduce.

**Author:** Zara Khan  
MSc Computer Science  
[Linkedin](https://www.linkedin.com/in/thezarakhan/)
