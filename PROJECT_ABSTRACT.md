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
a multi-model classification pipeline that combines traditional 
machine learning approaches (TF-IDF with Logistic Regression) 
with advanced neural architectures (LSTM and BERT-based models) 
to achieve high accuracy in distinguishing between reliable and 
misleading information.

The system processes textual features from news articles, 
including headlines, article body, and metadata, to generate 
probabilistic predictions about article credibility. We also 
develop interpretable outputs through attention visualization 
and feature importance analysis, enabling users to understand 
which linguistic patterns contribute to fake news identification.

## Scope of Work

### Technical Approach
| Phase | Method | Goal |
|-------|--------|------|
| Baseline | TF-IDF + Logistic Regression | Establish benchmark |
| Intermediate | LSTM | Capture sequential patterns |
| Advanced | Fine-tuned BERT | Deep contextual understanding |
| Final | Ensemble (all three) | Superior combined performance |

### System Components
- **Data Pipeline:** Preprocessing headlines, article body, metadata
- **Models:** TF-IDF, LSTM, BERT, Ensemble
- **Interpretability:** Attention visualization, feature importance
- **Interface:** Web app for real-world demonstration

## Split of Work

| Member | Responsibilities |
|--------|-----------------|
| Ritik Pravin Mota | TBD |
| Steve George | TBD |
| Sia Sopori | TBD |

## Dataset
TBD — Candidates:
- LIAR Dataset
- FakeNewsNet
- ISOT Fake News Dataset

## Evaluation Metrics
- Accuracy
- Precision
- Recall
- F1-Score
- Attention visualization for interpretability

## Related Work
- Shu et al. — hybrid model combining content + social context (~89% accuracy)
- Pérez-Rosas et al. — linguistic features (writing style, sentiment, syntax)
- Wang — LSTM networks outperform traditional ML by 8-12%

## Timeline
| Milestone | Target |
|-----------|--------|
| Data collection & preprocessing | TBD |
| Baseline model (TF-IDF + LR) | TBD |
| LSTM implementation | TBD |
| BERT fine-tuning | TBD |
| Ensemble & evaluation | TBD |
| Web interface | TBD |
| Final report | TBD |
