# 🚨 Disaster Tweet Classification Project

## 📌 Project Overview

**Competition**: [Kaggle NLP - Disaster Tweets](https://www.kaggle.com/c/nlp-getting-started)  
**Goal**: Classify tweets as disaster-related (1) or not (0)  
**Final F1-Score**: 0.80171 (Top 20% in competition)

### Key Features
- 🧹 Text preprocessing pipeline for noisy social media data
- 🔍 Comparative analysis of 4 ML algorithms
- ⚙️ Optimized SVM model with TF-IDF
- 🚀 Ready-to-use prediction pipeline

## 🏆 Performance Summary

| Metric        | Score   |
|--------------|---------|
| F1-Score     | 0.80171 |
| Accuracy     | 80.3%   |
| Precision    | 0.80    |
| Recall       | 0.71    |

## 🛠 Technical Implementation

### Model Architecture
```python
Pipeline(
    steps=[
        ('transformer', TextExtractor()),
        ('vectorizer', TfidfVectorizer()),
        ('classifier', SVC(C=1.3, degree=1))
    ]
)
