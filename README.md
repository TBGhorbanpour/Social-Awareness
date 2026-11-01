# 🌍 Social-Awareness

[![Jupyter Notebook](https://img.shields.io/badge/Jupyter-Notebook-F37626.svg?style=flat&logo=jupyter)](https://jupyter.org)
[![Python](https://img.shields.io/badge/Python-3.8%2B-blue.svg?style=flat&logo=python)](https://www.python.org)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

## 📖 About This Project

**Social-Awareness** is a comprehensive data science and Natural Language Processing (NLP) project designed to analyze social media data (specifically tweets). The project provides an end-to-end pipeline for extracting, cleaning, and analyzing tweet data to uncover social trends, sentiments, topics, and community structures. 

Given the use of specialized tools like **DadmaTools**, this pipeline is particularly well-suited for **Persian (Farsi) text analysis**, though the methodologies can be adapted to other languages.

## 📋 Table of Contents

- [About This Project](#-about-this-project)
- [Pipeline & Workflow](#-pipeline--workflow)
- [Project Structure](#-project-structure)
- [Dataset](#-dataset)
- [Prerequisites & Installation](#-prerequisites--installation)
- [How to Run](#-how-to-run)
- [Contributing](#-contributing)
- [Author](#-author)

## 🔄 Pipeline & Workflow

The repository is organized as a step-by-step analytical pipeline. It is recommended to run the notebooks in the following order:

1. **Data Extraction**: `Extract_tweets_by_tweeds.ipynb` – Scrapes or extracts raw tweet data.
2. **Filtering**: `PoliticalTweetFilter.ipynb` – Filters the dataset to isolate politically relevant or specific subsets of tweets.
3. **Preprocessing**: 
   - `Initial_Cleanup_.ipynb` – Basic data cleaning (handling missing values, removing duplicates, etc.).
   - `DadmaTools_Preprocess_.ipynb` – Advanced NLP preprocessing (tokenization, lemmatization, stopword removal) using the DadmaTools Persian NLP toolkit.
4. **NLP & Analysis**:
   - `NER.ipynb` – Named Entity Recognition to identify key people, organizations, and locations.
   - `Topic_Modeling.ipynb` – Discovers abstract topics within the tweet corpus (e.g., using LDA or similar methods).
   - `Location_based_topic_modeling.ipynb` – Extends topic modeling by incorporating geolocation data.
   - `Sentiment_Analysis.ipynb` – Classifies tweets into positive, negative, or neutral sentiments.
5. **Advanced Analysis**: `Community_Detection.ipynb` – Identifies clusters or communities within the data (e.g., user interaction networks or topic-based clusters).
6. **Visualization**: `Charts.ipynb` – Generates insightful charts and graphs to visualize the findings from the analysis steps.

## 📁 Project Structure

```text
Social-Awareness/
│
├── Data/                          # Directory containing the dataset (e.g., Dataset.csv via Git LFS)
├── Extract_tweets_by_tweeds.ipynb # Step 1: Data extraction
├── PoliticalTweetFilter.ipynb     # Step 2: Data filtering
├── Initial_Cleanup_.ipynb         # Step 3a: Basic data cleaning
├── DadmaTools_Preprocess_.ipynb   # Step 3b: NLP preprocessing (Persian)
├── NER.ipynb                      # Step 4a: Named Entity Recognition
├── Topic_Modeling.ipynb           # Step 4b: General topic modeling
├── Location_based_topic_modeling.ipynb # Step 4c: Geospatial topic modeling
├── Sentiment_Analysis.ipynb       # Step 4d: Sentiment classification
├── Community_Detection.ipynb      # Step 5: Network/community analysis
├── Charts.ipynb                   # Step 6: Data visualization
├── .gitattributes                 # Git LFS configuration
└── README.md                      # Project documentation
