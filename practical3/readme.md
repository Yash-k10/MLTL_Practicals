# Sentiment Analysis Practical

**Student Name:** Yash Kapse
**Technology Used:** HTML, JavaScript, TensorFlow.js (CDN)

---

## Overview

Sentiment Analysis is a Natural Language Processing (NLP) technique used to determine whether a sentence expresses **positive or negative emotion**.
This project demonstrates sentiment classification using **TensorFlow.js directly in the browser**.

---

## Task 1: Train Sentiment Classifier

* A small dataset of **positive and negative sentences** is created.
* The sentences are converted into **numerical vectors**.
* A **Neural Network model** is trained using TensorFlow.js to classify sentiment.

---

## Task 2: Test Custom Sentences

* The trained model accepts **user input sentences**.
* The system predicts **Positive or Negative sentiment**.
* A **confidence score** is displayed to show prediction probability.

Example:

Input:
`I love this product`

Output:
Positive 😊 (Confidence: 92%)

---

## Task 3: Compare Dense vs RNN

Two models are trained:

* **Dense Neural Network**
* **Recurrent Neural Network (RNN)**

Both models analyze the same input sentence and their **predictions and confidence scores are compared**.

| Model         | Characteristic            |
| ------------- | ------------------------- |
| Dense Network | Simple and fast           |
| RNN           | Understands word sequence |

RNN generally performs **better for text-based tasks**.

---

## Conclusion

This practical demonstrates how **Neural Networks can be used for sentiment analysis** in the browser using TensorFlow.js.
The comparison shows that **RNN models capture text context better than simple dense networks**.

---

⭐ Built using **TensorFlow.js + CDN**
