# 📊 Elon Musk Tweet Sentiment Analysis: Before vs After Acquiring X (Twitter)

This repository contains an NLP-based sentiment analysis of Elon Musk's tweets before and after his acquisition of X (formerly Twitter). The study provides insight into how the tone and sentiment of his tweets evolved.

Using a dataset of Elon Musk’s tweets and applying **TextBlob** sentiment analysis, the project classifies tweets into **positive**, **neutral**, and **negative** categories. It further visualizes sentiment trends and word usage patterns across two time periods—**before** and **after October 10, 2022** (the acquisition date).

---

## 🔧 Techniques Used

- **TextBlob** for sentiment polarity classification
- **Pandas & Seaborn** for data manipulation and visualization
- **Matplotlib & WordCloud** for plot generation
- **Regular Expressions** for text cleaning

---

## 📅 Dataset

- **Source**: Public Google Sheets containing Elon Musk’s tweets  
- **Format**: CSV (downloaded via `pandas.read_csv` from a public link)  
- **Key Columns**:  
  - `createdAt`: Timestamp of each tweet  
  - `fullText`: Text content of the tweet  

Tweets were divided into two periods:
- `before`: Before October 10, 2022
- `after`: On or after October 10, 2022

---

## 🧠 Sentiment Analysis Method

Each tweet was assigned a sentiment based on **TextBlob polarity**:
- `> +0.1` → Positive  
- `< -0.1` → Negative  
- Otherwise → Neutral  

A new `sentiment` column was created along with `sentiment_score` mapping:
- Positive → `1`
- Neutral → `0`
- Negative → `-1`

---

## 📈 Visualizations

### 🟣 Sentiment Distribution (Violin Plot)

Shows how sentiment scores are distributed in both periods:

![Violin Plot](https://github.com/JHK0723/musk-x-nlp-analysis/blob/ef2c6570740ebe9a44effbc6ba209688bd6ef6c8/violinplotnlpelon.png)

---

### ☁️ Word Clouds

Visual representation of the most frequent words in tweets:

![Violin Plot](https://github.com/JHK0723/musk-x-nlp-analysis/blob/ef2c6570740ebe9a44effbc6ba209688bd6ef6c8/wordcloudnlpelon.png)

## 📝 Summary Report

> 📌 **Sentiment Comparison Summary**

Before the acquisition:
- Total tweets: **18,816**
- Positive: **7,150 tweets (38.0%)**
- Neutral: **10,200 tweets (54.2%)**
- Negative: **1,466 tweets (7.8%)**

After the acquisition:
- Total tweets: **36,283**
- Positive: **14,058 tweets (38.7%)**
- Neutral: **18,362 tweets (50.6%)**
- Negative: **3,863 tweets (10.6%)**

> ✅ **Observation**: While positivity remained mostly stable, there was a noticeable uptick in negative sentiment after the acquisition, alongside a decline in neutrality, indicating a more polarized public reaction in the post-acquisition phase..

---

Note: Due to the notebook's output size and complexity, GitHub may not render it properly and display an "Unable to render code block" message. For a better experience, view the notebook via nbviewer.org/github/JHK0723/musk-x-nlp-analysis/blob/main/NLP_analysis_Elon_Musk_tweets_before,during_and_after_ownership_of_X.ipynb.

## 🚀 How to Run

1. Clone the repo:
   ```bash
   git clone https://github.com/yourusername/elon-tweet-nlp.git
   cd elon-tweet-nlp

   
