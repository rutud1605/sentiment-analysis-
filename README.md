# 📌 Sentiment Analysis on Yelp Reviews

## 🔍 Introduction
In the digital era, customer reviews on platforms like Yelp provide valuable insights into user satisfaction and business performance. This project focuses on Sentiment Analysis to classify Yelp reviews into positive, neutral, or negative categories using deep learning techniques.

We implemented and compared two models:

- LSTM (Long Short-Term Memory) – A recurrent neural network for sequential text processing.
- DistilBERT – A lightweight Transformer model for context-aware text classification.

## 🎯 Objectives
- Analyze customer sentiments from Yelp restaurant reviews.
- Compare LSTM and DistilBERT models for sentiment classification.
- Improve sentiment prediction accuracy with advanced NLP techniques.

## 📊 Dataset
We used a 6,000-review dataset from Yelp, focusing on restaurant businesses. The dataset includes:

- Business ID – Unique identifier for each restaurant.
- Text – The actual customer review.
- Stars (1-5) – Ratings converted into sentiment labels:
- Positive (4-5 stars)
- Neutral (3 stars)
- Negative (1-2 stars)
  
## 🛠 Data Preprocessing
- Text Cleaning – Lowercasing, punctuation removal, and lemmatization.
- Tokenization – Converting words into numerical representations.
- Padding – Standardizing input length for LSTM.

## 🧠 Model Architectures
📌 LSTM Model
A deep learning model designed for sequential text analysis:

- Layers: Embedding, LSTM, Fully Connected, Softmax
- Optimizer: Adam
- Loss Function: Cross-Entropy Loss
- Training: Backpropagation with tokenized review sequences

## 📈 Results & Discussion
- 📌 DistilBERT outperformed LSTM, achieving 77% accuracy compared to LSTM’s 65%.
- 📌 LSTM struggled with training efficiency due to sequential data processing.
- 📌 DistilBERT handled contextual understanding better, leading to higher accuracy.
- 📌 More data would further enhance DistilBERT's performance, making it an ideal choice for large-scale sentiment analysis.

## 🛠 Technologies Used
- Python, TensorFlow, PyTorch, Hugging Face Transformers
- Natural Language Processing (NLP) – Tokenization, Lemmatization, Padding
- Deep Learning – LSTM, Transformer-based DistilBERT
- Scikit-learn – Performance evaluation (Precision, Recall, F1-Score)
- Jupyter Notebooks & Pandas – Data preprocessing & visualization
