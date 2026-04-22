# Project Abstract

## Project Title
Fake News Detection System

## Abstract
The proliferation of fake news on social media platforms poses
a significant threat to informed public discourse, democratic
processes, and individual decision-making. False information
spreads six times faster than factual news on social media,
and exposure to misinformation can significantly influence
public opinion on critical issues such as elections, public
health, and social policies.

This project develops an automated fake news detection system
using natural language processing and deep learning techniques
to classify news articles as authentic or fabricated. We build
a multi-model classification pipeline combining traditional
machine learning (TF-IDF with Logistic Regression) with advanced
neural architectures (LSTM and fine-tuned RoBERTa transformer)
to achieve high accuracy in distinguishing reliable from
misleading information.

All three models were trained on the ISOT Fake News Dataset
(44,898 articles) and evaluated on both a held-out test set
and an independent FakeNewsNet dataset to assess cross-domain
generalizability. Our key finding is that despite RoBERTa
achieving near-perfect in-distribution accuracy (~100%), all
three models achieve identical 97% F1 on FakeNewsNet, suggesting
simpler models learn equally transferable linguistic signals.
We also provide model interpretability through SHAP global
feature importance and LIME instance-level explanations, and
deploy a real-time web interface using Gradio.

## Scope of Work

### Technical Approach
| Phase | Method | Goal |
|-------|--------|------|
| Baseline | TF-IDF + Logistic Regression | Establish benchmark |
| Intermediate | LSTM | Capture sequential patterns |
| Advanced | Fine-tuned RoBERTa | Deep contextual understanding |
| Explainability | SHAP + LIME | Interpret model predictions |
| Deployment | Gradio Web Interface | Real-world demonstration |

### System Components
- **Data Pipeline:** Reuters bias detection & removal, URL stripping,
  whitespace normalization, title + body concatenation
- **Models:** TF-IDF + LR, LSTM, RoBERTa (roberta-base, 125M parameters)
- **Evaluation:** In-distribution (ISOT) + cross-dataset (FakeNewsNet)
- **Interpretability:** SHAP global feature importance, LIME instance explanations
- **Interface:** Gradio web app with real-time predictions from all three models

## Split of Work

| Member | Responsibilities |
|--------|-----------------|
| Ritik Pravin Mota | Evaluation strategy, cross-dataset generalization testing, confusion matrix analysis, model comparison methodology, SHAP/LIME interpretation, analysis & discussion sections |
| Steve George | Project coordination, proposal, GitHub repository setup, final report authoring, notebook completeness (missing evaluations, training curves, model comparison table, bug fixes) |
| Sia Sopori | Core technical implementation — all three models, data pipeline, preprocessing, SHAP/LIME analysis, Gradio deployment, Kaggle GPU training, codebase |

## Dataset
- **Training/Evaluation:** ISOT Fake News Dataset — 44,898 articles
  (23,481 fake / 21,417 real), 2016–2017, sourced from Reuters and
  PolitiFact-flagged sites. Split: 80% train / 10% val / 10% test.
- **Cross-dataset Test:** FakeNewsNet (GonzaloA/fake_news on HuggingFace)
  — 8,117 articles from diverse sources, used for generalizability testing.

## Results

| Model | ISOT Accuracy | ISOT F1 | FakeNewsNet F1 |
|-------|--------------|---------|----------------|
| TF-IDF + Logistic Regression | 98% | 98% | 97% |
| LSTM | 98% | 98% | 97% |
| RoBERTa | ~100% | ~100% | 97% |

**Key finding:** All three models achieve identical 97% F1 on FakeNewsNet
despite RoBERTa's apparent ISOT advantage — suggesting the gap reflects
dataset-specific patterns rather than superior language understanding.

## Evaluation Metrics
- Accuracy, Precision, Recall, F1-Score
- Confusion matrices per model
- Cross-dataset generalization (FakeNewsNet)
- SHAP feature importance scores
- LIME instance-level explanations

## Related Work
- Shu et al. (2020) — FakeNewsNet: hybrid model combining content +
  social context (~89% accuracy)
- Pérez-Rosas et al. (2018) — linguistic features (writing style,
  sentiment, syntax) achieve 76% accuracy, comparable to humans
- Wang (2017) — LIAR dataset; LSTM networks outperform traditional
  ML by 8–12%
- Liu et al. (2019) — RoBERTa: robustly optimized BERT pretraining,
  125M parameters, pretrained on 160GB text
