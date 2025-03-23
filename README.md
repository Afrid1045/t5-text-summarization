# 🧠 T5 Text Summarization – Mini Project

This project demonstrates how to use the T5 Transformer model for **text summarization** using Hugging Face 🤗 Transformers. It includes hands-on steps for running inference, fine-tuning on custom data, and evaluating the fine-tuned model.

---

## 🔍 Objective

- Understand **sequence-to-sequence** (text-to-text) modeling using T5
- Learn how to tokenize, generate summaries, and decode outputs
- Fine-tune a pretrained model and visualize training loss
- Run inference on unseen text using the fine-tuned model

---

## 🧱 Folder Structure

t5_text_summarization/ │ ├── 01_intro_and_setup.ipynb ← Concept + basic testing ├── 02_tokenization_and_basics.ipynb← Tokenizing & decoding walkthrough ├── 03_inference_baseline.ipynb ← Summarization using pretrained model ├── 04_fine_tuning.ipynb ← Training loop, loss logging, model save ├── 05_evaluation.ipynb ← Load trained model & run new inference │ ├── results/ │ └── t5_finetuned/ ← Fine-tuned model & tokenizer

yaml
Copy
Edit

---

## ⚙️ How to Run

1. Clone the repo
2. Install required packages:
   ```bash
   pip install torch transformers datasets matplotlib
Run notebooks in order:

01_intro_and_setup.ipynb → 05_evaluation.ipynb

✨ Example Output
Input:

summarize: Artificial Intelligence is transforming healthcare...

Generated Summary:

AI-powered tools can analyze vast medical data, assist in diagnostics, and recommend personalized treatments.

📚 What I Learned
How T5 models handle summarization as a text-to-text problem

How tokenization works and why decoding is needed

How to fine-tune a Transformer on small datasets

Importance of beam search, padding, and decoding strategies

📌 Next Steps
Try other summarization datasets (e.g., XSum, CNN-DailyMail)

Experiment with longer models like t5-base or t5-large

Add Streamlit or Gradio frontend for live summarization