# PropagandaScope

PropagandaScope is a machine learning toolkit for detecting propaganda techniques in news articles. The project implements multiple models for both **technique classification** and **span detection**, addressing the SemEval‑2020 Task 11 challenge.

This project was developed as part of the *Advanced Natural Language Engineering (G5114)* module.

## 🎯 Tasks

### Task 1: Technique Classification
Classify a known span of text into one of 9 propaganda techniques.

- ✅ **TF-IDF + Logistic Regression** (baseline)
- ✅ **BERT Sequence Classification**

### Task 2: Span Detection + Technique Classification
Identify the spans in text where propaganda occurs and label them.

- ✅ **BiLSTM-Softmax sequence labeling**
- ✅ **BERT Token Classification**

## 📊 Results Summary

| Model                         | Macro-F1 Score | Notes                          |
|------------------------------|----------------|--------------------------------|
| TF-IDF + Logistic Regression | 0.34           | Baseline method                |
| BERT Sequence Classification | 0.41           | Improved context understanding |
| BiLSTM Token Classification  | ~0.003         | Collapsed on class imbalance   |
| BERT Token Classification    | ~0.009         | Slightly better, still weak    |

## 📦 Requirements

Install the dependencies via pip:

```bash
pip install -r requirements.txt
