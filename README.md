# 💬 Sentiment Analysis on Social Media using RoBERTa

This project applies Natural Language Processing (NLP) techniques to classify sentiment in social media comments related to music artists. The goal is to quantify public perception and analyze how sentiment correlates with engagement or revenue trends.

---

## 🧠 Project Overview

Understanding how fans feel about an artist can provide valuable insights for marketing, forecasting, and A&R strategies. In this project, we use state-of-the-art transformer models to analyze sentiment in Instagram and Twitter comments.

- ✅ Pretrained model: RoBERTa fine-tuned for sentiment analysis
- 🔍 Goal: Classify comments as **positive**, **neutral**, or **negative**
- 📊 Optional: Aggregate sentiment over time to use in forecasting models

---

## 📁 Dataset

The dataset contains real or synthetic social media comments related to artists, including:

- `artist_id`: unique artist identifier
- `comment`: social media comment text
- `date`: date of the comment (optional)
- `platform`: Instagram or Twitter

> 📁 An example dataset is available in the `data/` folder.

---

## 🤖 Model & Methodology

- We use the `cardiffnlp/twitter-roberta-base-sentiment` model from HuggingFace
- The model returns scores for `positive`, `neutral`, and `negative` classes
- Results are aggregated per artist or time period as needed

Steps:
1. Preprocess text (remove emojis, links, usernames, etc.)
2. Tokenize and feed into RoBERTa
3. Extract predicted label and confidence
4. Aggregate and visualize

---

## 📈 Example Output

| comment                                 | label     | confidence |
|-----------------------------------------|-----------|------------|
| "I love her new track so much!"         | positive  | 0.98       |
| "He's ok I guess."                      | neutral   | 0.73       |
| "Worst concert I've ever been to..."    | negative  | 0.96       |

---

## 📦 How to Run

1. Clone the repo:
   ```bash
   git clone https://github.com/tu-usuario/sentiment-analysis-social-media.git
   cd sentiment-analysis-social-media
