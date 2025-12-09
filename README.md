# 🧠 Project 07 — Incident Classification & SLA Risk Detection (NLP)

## 📌 Overview

This project builds an end-to-end NLP pipeline for **automatic classification of operational incidents** in logistics environments, with direct impact on:

- SLA monitoring  
- Risk reduction  
- Faster triage and prioritization  
- Operational decision-making efficiency  

The model analyzes textual descriptions of daily incidents (system failures, delays, route issues, vehicle unavailability, hub exceptions) and compares:

- **Traditional ML models** (TF-IDF + classifiers)  
- **Modern embedding-based or LLM-based classification approaches**

The objective is to determine **which pipeline provides the best balance between accuracy, interpretability, and operational applicability**.

## 🎯 Project Objectives

- Build an NLP classifier capable of interpreting incident descriptions.
- Structure a complete text-processing workflow.
- Compare ML approaches:
  - TF-IDF + Logistic Regression
  - TF-IDF + Random Forest
  - Embedding-based classification
- Evaluate metrics relevant for multiclass operational scenarios:
  - Accuracy
  - Recall per class
  - F1-score
  - Confusion Matrix
- Provide executive insights regarding SLA impact and operational risk.

## 📂 Repository Structure

project-07-incident-nlp-classification/
│
├── data/
│   ├── raw/                  # Unmodified source data
│   └── processed/            # Cleaned, vectorized data, TF-IDF, embeddings, splits
│
├── notebooks/
│   ├── study-version.ipynb   # Mentorship notebook (experiments, reasoning, testing)
│   └── final-version.ipynb   # Executive notebook (clean, clear, LinkedIn/GitHub-ready)
│
├── notes/
│   └── project-07-day1.md    # Technical diary and decisions log
│
├── README.md                 # This file
└── requirements.txt          # Environment dependencies

## 🛠️ Methodology (Summary)

### 1. Data Exploration
- Initial inspection of textual fields  
- Incident distribution  
- Length analysis  
- Basic cleaning and normalization  

### 2. NLP Preprocessing
- Lowercasing  
- Tokenization  
- Stopword removal  
- Lemmatization / stemming (as applicable)

### 3. Vectorization
- **TF-IDF** for classical models  
- **Embeddings** for semantic classification  
  - Sentence Transformers  
  - OpenAI embeddings (optional)

### 4. Modeling
- Logistic Regression  
- Random Forest  
- Embedding-based classifier (cosine similarity or fine-tuning)

### 5. Model Comparison
Evaluated via:

- Accuracy  
- Macro/micro F1  
- Per-class recall  
- Confusion matrix  
- Inference time  
- Operational robustness  

### 6. Executive Insights
- Patterns that most impact SLA  
- Critical incident categories  
- Bottlenecks in manual triage  
- How automation can reduce operational risk

## 📊 Results (to be filled after model execution)

This section will be completed after testing all approaches.

We will include:

- Model comparison table  
- Visual charts (confusion matrix, performance bars)  
- Key insights for operations and SLA management  

## 🚀 How to Run This Project

### 1. Install dependencies

```bash
pip install -r requirements.txt

jupyter notebook notebooks/study-version.ipynb
# or
jupyter notebook notebooks/final-version.ipynb


---

# ✅ **CELL 7 — Project Status**

```markdown
## 📝 Project Status

✔️ Repository created  
✔️ Corporate briefing received  
✔️ Initial structure defined  
🟡 In progress — Data exploration & NLP preprocessing  

## 🧭 Next Steps

- Load and explore real incident dataset  
- Create baseline models  
- Implement TF-IDF vectorization  
- Train classical ML classifiers  
- Implement embedding-based classification  
- Compare methods  
- Produce executive summary  
