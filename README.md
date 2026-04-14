# Fake News Detection System

![Python](https://img.shields.io/badge/Python-3.8+-blue)
![ML](https://img.shields.io/badge/ML-RoBERTa%20%7C%20LSTM%20%7C%20TF--IDF-green)
![Course](https://img.shields.io/badge/Course-CS%206140-red)

## Overview
An automated fake news detection system using machine learning 
and deep learning to classify news articles as authentic or 
fabricated. Built as part of CS 6140 (Machine Learning) at 
Northeastern University.

## Team
| Member | Email |
|--------|-------|
| Ritik Pravin Mota | mota.r@northeastern.edu |
| Steve George | george.ste@northeastern.edu |
| Sia Sopori | sopori.s@northeastern.edu |

## Approach
- **Baseline:** TF-IDF + Logistic Regression
- **Intermediate:** LSTM for sequential pattern capture
- **Advanced:** Fine-tuned RoBERTa transformer
- **Explainability:** SHAP + LIME analysis
- **Deployment:** Gradio web interface

## Results
| Model | ISOT Accuracy | FakeNewsNet F1 |
|-------|--------------|----------------|
| TF-IDF + LR | 98% | 97% |
| LSTM | 98% | 97% |
| RoBERTa | 100% | 97% |

## Repository Structure
```
Fake-News-Detection-System/
├── machlearning.ipynb
├── README.md
└── PROJECT_ABSTRACT.md
```

## Course
CS 6140 - Machine Learning  
Northeastern University, Spring 2026
