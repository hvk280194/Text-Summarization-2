# 📘 Advanced Text Summarization using BART Transformers

This repository contains a **recruiter-ready, advanced text summarization project** using **BART (facebook/bart-large-cnn)**. The notebook demonstrates a complete NLP workflow, from data preprocessing to model fine-tuning, evaluation, and inference.

---

## 🚀 Project Overview

The goal of this project is to build an **abstractive text summarization system** that can generate concise summaries from long news articles. The project includes:

- Advanced preprocessing (cleaning, sliding window for long articles)
- Optional extractive + abstractive hybrid summarization
- Fine-tuning with gradient accumulation, learning rate scheduling, early stopping
- Evaluation using **ROUGE** and **BERTScore**
- Beam search and top-k/top-p inference for improved summaries
- Visualization of generated summaries and metrics
- Model saving and reloading for deployment
- Optional: interactive **Streamlit interface** for live text summarization

---

## 📂 Dataset

- **CNN/DailyMail** (version 3.0.0)
- Alternatively, you can experiment with **XSum**
- Notebook uses a small subset for demo, designed to scale to full datasets

---

## 🔧 Features & Highlights

1. **Data Preprocessing**
   - Removes HTML tags and extra whitespace
   - Splits long articles into chunks
   - Optional extractive sentence selection

2. **Model Setup**
   - Uses `facebook/bart-large-cnn` from HuggingFace
   - GPU support if available

3. **Training**
   - Gradient accumulation
   - Early stopping on validation ROUGE
   - Mixed-precision support

4. **Inference**
   - Beam search with length penalty
   - Top-k / top-p sampling
   - Compare multiple decoding strategies

5. **Evaluation**
   - ROUGE-1, ROUGE-2, ROUGE-L
   - BERTScore for semantic similarity
   - Visual comparison of generated vs reference summaries

6. **Visualization**
   - Summary length vs article length
   - ROUGE score bar charts
   - Side-by-side original vs generated summaries

7. **Deployment**
   - Model and tokenizer saved for inference
   - Optional interactive Streamlit interface

---

## 📝 How to Run

1. Clone the repository:

```bash
git clone https://github.com/<your-username>/Advanced-BART-Text-Summarization.git
cd Advanced-BART-Text-Summarization
