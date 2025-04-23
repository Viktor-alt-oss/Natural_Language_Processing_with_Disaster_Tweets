# Disaster Tweet Classification Project
Project Banner Replace with actual banner image

##📌 Project Overview
This project tackles Kaggle's "Natural Language Processing with Disaster Tweets" competition, developing a machine learning model to classify whether tweets are about real disasters (1) or not (0). The solution achieved 0.80171 F1-score on the competition's test set.

## Key Features:

Text preprocessing pipeline for noisy tweet data

Comparative analysis of multiple ML algorithms

Optimized SVM classifier with TF-IDF vectorization

Ready-to-use prediction pipeline

## 🏆 Performance Summary
Metric	Score
Competition F1-Score	0.80171
Test Accuracy	80.3%
Precision	0.80
Recall	0.71
🛠 Technical Implementation
Model Architecture

graph LR
    A[Raw Tweet] --> B[Text Extraction]
    B --> C[TF-IDF Vectorization]
    C --> D[SVM Classifier]
    D --> E[Prediction]
---
## 🚀 Описание проекта
### Данные
В наличии три ключевых файла:
- `train.csv` — обучающий набор с размеченными твитами.
- `test.csv` — тестовый набор для предсказаний.
- `sample_submission.csv` — пример файла для отправки на Kaggle.

**Структура данных**:
- `id` — уникальный идентификатор твита.
- `text` — текст твита.
- `location` — место отправки (может быть пустым).
- `keyword` — ключевое слово из твита (может быть пустым).
- `target` — бинарная метка (`1` = катастрофа, `0` = нет; только в `train.csv`).

### Пример проблемы
Твит:  
*"На улице всё в огне! #хаос"*  
Может означать как реальный пожар, так и метафорическое выражение. Задача модели — корректно классифицировать такие случаи.
