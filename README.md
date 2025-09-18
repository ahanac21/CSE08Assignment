# Sentiment Classification: LSTM vs BERT

This repository contains the Colab notebook for our project on sentiment classification using the IMDB movie review dataset. We implement and compare two models — a Long Short-Term Memory (LSTM) network and a transformer-based BERT model — to analyze their strengths, weaknesses, and trade-offs.

## Contents
- `sentiment_analysis_pipeline.ipynb`: End-to-end pipeline covering:
  - Data loading and preprocessing  
  - Model building (LSTM and BERT)  
  - Training, evaluation, and error analysis  

## Running the Notebook
Click the badge below to open the notebook directly in Google Colab:

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/your-username/your-repo-name/blob/main/sentiment_analysis_pipeline.ipynb)

*(Replace `your-username` and `your-repo-name` with your actual GitHub info.)*

## Dataset
We use the IMDB movie reviews dataset (25,000 training + 25,000 test samples) with balanced positive and negative labels, accessed through the Hugging Face `datasets` library.

## Results Summary
- **LSTM Model**  
  - Accuracy: 82.2%  
  - Macro F1-score: 0.82  
  - Stronger at identifying negative reviews but weaker on positives (recall = 0.73)  
  - Fast training (< 5 minutes total), lightweight but less robust.  

- **BERT Model**  
  - Accuracy: 92.1%  
  - Macro F1-score: 0.92  
  - Balanced performance across both classes (precision/recall ≈ 0.91–0.93)  
  - Training costlier (~57 minutes for 3 epochs), but delivers state-of-the-art performance.  

## Key Insights
- LSTMs are efficient and practical for quick baselines.  
- BERT provides significantly better accuracy and balanced predictions but requires more compute.  
- The trade-off between performance and efficiency is crucial depending on application needs.  

---

