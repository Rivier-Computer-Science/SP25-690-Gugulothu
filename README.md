# SP25-690-Gugulothu

# Deep Learning-Based Sentiment Analysis of User Reviews

##  Overview

This project implements a sentiment analysis system that classifies IMDB movie reviews as **positive** or **negative** using deep learning techniques.

The project compares:

* A baseline **LSTM model**
* A transformer-based **BERT model**

---

##  Objective

To evaluate and compare the performance of traditional sequence models (LSTM) with modern transformer-based models (BERT) for text classification tasks.

---

##  Dataset

* **Dataset**: IMDB Movie Reviews Dataset
* **Size**: 50,000 labeled reviews
* **Classes**: Balanced (Positive / Negative)
* **Source**: Hugging Face `datasets` library

---

##  Models Implemented

###  1. LSTM (Baseline Model)

* Embedding layer + LSTM
* Trained from scratch
* Captures sequential dependencies
* Serves as a baseline for comparison

---

###  2. BERT (Advanced Model)

* Pretrained transformer model
* Fine-tuned on IMDB dataset
* Captures contextual and bidirectional relationships in text

---

##  Tech Stack

* Python
* PyTorch
* Hugging Face Transformers
* Scikit-learn
* Google Colab (GPU)

---

## 📂 Project Structure

```
SP25-690-Gugulothu/
│── Sentiment_Analysis_Project.ipynb
│── README.md
│── DATA.md
│── config.yaml
│── environment.yml
│── requirements.txt


```
---

## 📈 Evaluation Metrics

The models are evaluated using:

* Accuracy
* Precision
* Recall
* F1-score

---

##  Results

| Model              | Accuracy |
| ------------------ | -------- |
| LSTM (Baseline)    | 0.518    |
| BERT (Transformer) | 0.904    |

---

##  Key Insights

* BERT significantly outperforms LSTM due to its ability to understand contextual relationships in text.
* LSTM struggles with long-range dependencies and complex sentence structures.
* Transformer-based models are more effective for modern NLP tasks.

---

##  Failure Analysis

Common challenges observed:

* **LSTM limitations:**

  * Poor handling of long reviews
  * Difficulty with negation (e.g., "not bad")
  * Limited contextual understanding

* **BERT limitations:**

  * Sarcasm detection
  * Ambiguous language

---

##  Ethics & Limitations

* Possible bias in training data
* Model may not generalize to all domains
* Not suitable for critical decision-making without further validation

---

##  Reproducibility

* Fixed dataset splits
* Clear training scripts provided
* End-to-end pipeline included

---

##  References

* Devlin et al., 2019 – BERT: Pre-training of Deep Bidirectional Transformers
* Hugging Face Transformers Documentation
* IMDB Dataset

---

##  Author

Thirupathi Gugulothu
