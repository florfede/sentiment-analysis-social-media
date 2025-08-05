# 💬 Sentiment Analysis on Social Media using RoBERTa

This project uses Natural Language Processing (NLP) to classify the sentiment of comments from Instagram and Twitter about music artists. The goal is to monitor fan perception and extract actionable insights.

---

## 🧠 Project Overview

Understanding fan sentiment helps identify trends, assess artist reputation, and enhance decision-making in marketing and A&R.

We use a transformer-based model to label comments as:

- ✅ Positive
- ➖ Neutral
- ❌ Negative

---

## 🤖 Model

- **Model used**: `cardiffnlp/twitter-roberta-base-sentiment` from HuggingFace
- **Type**: Fine-tuned RoBERTa for sentiment classification
- **Pipeline**:
  1. Clean text (remove URLs, emojis, tags)
  2. Tokenize
  3. Predict label and confidence

---

## 📁 Folder Structure

```
sentiment-analysis-social-media/
│
├── data/              # Example comment data
├── notebooks/         # Sentiment analysis notebook
├── outputs/           # Predictions and plots
├── src/               # Text preprocessing scripts (optional)
├── requirements.txt   # Python dependencies
└── README.md
```

---

## 📊 Example Output

| Comment                                 | Label    | Confidence |
|-----------------------------------------|----------|------------|
| I love this song so much!               | Positive | 0.96       |
| Not bad, not great.                     | Neutral  | 0.72       |
| What a terrible performance 😤          | Negative | 0.94       |

---

## 🧪 How to Run

1. Clone the repo:
```bash
git clone https://github.com/tu-usuario/sentiment-analysis-social-media.git
cd sentiment-analysis-social-media
```

2. Install dependencies:
```bash
pip install -r requirements.txt
```

3. Run the notebook:
```bash
jupyter notebook notebooks/sentiment_analysis_roberta.ipynb
```

---

## 📚 Tech Stack

- Python
- HuggingFace Transformers
- RoBERTa
- pandas / numpy
- matplotlib / seaborn

---

## 👩‍💻 Author

**Florencia Federico**  
Data & Machine Learning Engineer  
[LinkedIn](https://www.linkedin.com/in/florenciafederico88/)
