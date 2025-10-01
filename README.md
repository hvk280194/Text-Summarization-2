# 📘 Advanced Text Summarization using BART Transformers

This repository contains a **recruiter-ready, advanced text summarization project** using **BART (facebook/bart-large-cnn)**. The notebook demonstrates a complete NLP workflow, from data preprocessing to model fine-tuning, evaluation, and inference.

---

## 🚀 Project Overview

The goal of this project is to build an **abstractive text summarization system** that generates concise summaries from long news articles. The project includes:

- Advanced preprocessing with cleaning and sliding window for long articles
- Optional extractive + abstractive hybrid summarization
- Fine-tuning with gradient accumulation, learning rate scheduling, and early stopping
- Evaluation using **ROUGE** and **BERTScore**
- Beam search and top-k/top-p inference for improved summaries
- Visualization of generated summaries and metrics
- Model saving and reloading for deployment
- Optional: interactive **Streamlit interface** for live text summarization

---

## 📂 Dataset

- **CNN/DailyMail** (version 3.0.0)  
- Optionally, you can experiment with **XSum**  
- Notebook uses a small subset for demonstration, designed to scale to full datasets

---

## 🔧 Features & Highlights

- **Data Preprocessing**: Removes HTML tags, extra whitespace, splits long articles into chunks, optional extractive sentence selection  
- **Model Setup**: Uses `facebook/bart-large-cnn` from HuggingFace, GPU support if available  
- **Training**: Gradient accumulation, early stopping on validation ROUGE, mixed-precision support  
- **Inference**: Beam search with length penalty, top-k / top-p sampling, comparison of decoding strategies  
- **Evaluation**: ROUGE-1, ROUGE-2, ROUGE-L, BERTScore, visual comparison of generated vs reference summaries  
- **Visualization**: Summary length vs article length, ROUGE score bar charts, side-by-side text comparison  
- **Deployment**: Model and tokenizer saved for inference, optional Streamlit interface  

---

## 📝 How to Run

Clone the repository:

```bash
git clone https://github.com/<your-username>/Advanced-BART-Text-Summarization.git
cd Advanced-BART-Text-Summarization
