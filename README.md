# Fiction vs. Non-Fiction Book Classifier 📚

This repository contains the final project for **SI630: Natural Language Processing** at the University of Michigan.

## 📌 Project Overview

The goal of this project is to automatically classify books as either *fiction* or *non-fiction* using only short Wikipedia-style summaries. Rather than requiring full-text documents, this system uses concise, reader-style summaries as input — making it practical, efficient, and scalable for use in real-world digital libraries and recommendation systems.

## 🧠 Methodology

The project explores and compares two approaches:

1. **Traditional Machine Learning**:  
   - Preprocessing with TF-IDF vectorization  
   - Classifiers: Logistic Regression, SVM, and Random Forest  
2. **Deep Learning with BERT**:  
   - Fine-tuning `bert-base-uncased` from Hugging Face  
   - Tokenization with max sequence length 128  
   - Evaluation using macro F1-score and accuracy

All models were trained on a dataset of 10,000 Wikipedia-derived book summaries, equally split between fiction and non-fiction.

## 📊 Results

| Model                 | Accuracy | Macro F1 |
|----------------------|----------|----------|
| Logistic Regression  | 97.5%    | 0.975    |
| SVM                  | 97.3%    | 0.973    |
| Random Forest        | 97.1%    | 0.971    |
| BERT (fine-tuned)    | **99.6%**| **0.996**|

While traditional models performed very strongly, the BERT-based transformer model outperformed all baselines, especially on more ambiguous summaries.

## 🔗 Acknowledgments

- This project was completed as part of SI630 at the University of Michigan.  

