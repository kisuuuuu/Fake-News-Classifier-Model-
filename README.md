# 📰 Fake News Article Detector

A machine learning project that leverages **BERT (Bidirectional Encoder Representations from Transformers)** to accurately detect fake news articles from real ones. Developed as a part of a Modeling and Simulation course, this project addresses the critical issue of misinformation on digital platforms, particularly in the context of the Philippines.

## Project Overview

Fake news is a growing concern in today’s digital age, especially on social media platforms like Facebook. This project aims to build a reliable and efficient fake news classification system using Natural Language Processing (NLP) techniques and transformer-based models.

-  **Model Used**: BERT (Fine-tuned for binary text classification)
-  **Accuracy Achieved**: 90% (Prototype 6, 150 epochs on T4 GPU)
-  **Tools & Libraries**: Python, PyCaret, NumPy, Pandas, Scikit-Learn, Matplotlib, Google Colab

## Dataset

The model is trained and evaluated on datasets from [FakeNewsNet (KaiDMML GitHub)](https://github.com/KaiDMML/FakeNewsNet), specifically:
- `politifact_real.csv`
- `politifact_fake.csv`

The data was preprocessed, merged, and stratified for training, validation, and testing.

## Methodology

1. **Preprocessing**: Tokenization and encoding using BERT tokenizer.
2. **Model Training**:
   - Fine-tuned BERT using supervised learning.
   - Optimized using AdamW optimizer.
   - Iteratively trained across six prototypes with increasing complexity and resources.
3. **Evaluation**: Classified using precision, recall, and F1-score metrics. Final model achieved **90% accuracy** with balanced performance.
4. **Deployment Script**: A classification function was created to detect fake news from input URLs.

## How to Run

1. Clone this repository:
   ```bash
   git clone https://github.com/yourusername/fake-news-detector.git
   cd fake-news-detector
