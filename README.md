# Sentiment Analysis of Public Opinion on the Indonesian Academic Ability Test (TKA) Policy Using IndoBERT

This repository contains the dataset, source code, and experimental results used in the undergraduate thesis:

> **Sentiment Analysis of X Users Toward the Senior High School Academic Ability Test (Tes Kemampuan Akademik/TKA) Policy Using IndoBERT**

This research was conducted as a partial fulfillment of the requirements for obtaining a Bachelor's Degree in Mathematics at Universitas Negeri Yogyakarta.

---

## 📖 Research Overview

The implementation of the **Academic Ability Test (Tes Kemampuan Akademik/TKA)** has generated diverse public opinions on social media. This study aims to analyze public sentiment expressed on the X platform (formerly Twitter) regarding the TKA policy for senior high schools.

A sentiment classification model based on **IndoBERT (indobenchmark/indobert-base-p2)** was fine-tuned to classify tweets into three sentiment categories:

- Positive
- Neutral
- Negative

The research employs a combination of **pseudo-labeling** and **manual annotation** to construct a high-quality labeled dataset before model training.

---

## 📊 Dataset

- Source : X (Twitter)
- Language : Indonesian
- Data Collection Period : May 25, 2025 – January 5, 2026
- Total Tweets : **4,439**
---

## ⚙️ Methodology

The research workflow consists of the following stages:

1. Data Crawling
2. Text Preprocessing
   - Case Folding
   - Cleaning
   - Text Normalization
3. Hybrid Data Labeling
   - Pseudo-labeling
   - Manual Annotation of Low-Confidence Data
5. Dataset Splitting
6. Fine-tuning IndoBERT
7. Model Evaluation
---

## 🧠 Model

Model used:

```
indobenchmark/indobert-base-p2
```

Training configuration:

| Parameter | Value |
|-----------|-------|
| Optimizer | AdamW |
| Learning Rate | 2e-5 |
| Batch Size | 16 |
| Epoch | 4 |
| Weight Decay | 0.05 |
| Loss Function | Weighted Cross Entropy |

---
## 💻 Environment

- Python 3.12.13
- Google Colaboratory
- NVIDIA Tesla T4 GPU

Main Libraries:

- transformers
- torch
- scikit-learn
- pandas
- numpy
- matplotlib
- wordcloud
- Tweet-Harvest

---
## 👩‍🎓 Author

**Keisha Kayana Aptadhea**

---

## ⚠️ Disclaimer

The dataset was collected from publicly available posts on X (Twitter) and is shared solely for academic and research purposes. Users are expected to comply with the platform's terms of service and applicable ethical guidelines when using the data.
