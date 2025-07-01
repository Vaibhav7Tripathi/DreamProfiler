# 🌙 DreamProfiler: Personalized AI-Powered Dream Interpretation

DreamProfiler is a memory-based AI system designed to interpret dreams through a **personalized and emotionally grounded lens**. Unlike generic LLMs, it learns from a user’s past dreams to provide context-aware and psychologically meaningful insights.

---

## 📌 Project Overview

🔍 **What it does:**
- Detects and explains **dominant emotions** and their intensity  
- Identifies and remembers **recurring symbols** and metaphors  
- Tracks **emotional arcs and dream evolution** over time  
- Outputs interpretations in a **thoughtful, structured format**

🧠 **How it's different:**
- Builds **user-specific dream profiles**  
- Works **offline** with local models  
- Focuses on **emotion entropy** and **symbol consistency** instead of rigid NLP accuracy metrics  

---

## 💻 Setup & Dependencies

### ✅ Required Libraries

Install all dependencies using:

```bash
pip install transformers sentence-transformers matplotlib seaborn scikit-learn pandas

📁 Dataset Format
Make sure to pre-download a dream dataset with the following columns:

plaintext
Copy
Edit
dream_id, user_id, dream_text
You can use datasets like DreamBank or generate synthetic dreams using LLMs.

⚙️ Device Requirements
⚡ GPU Recommended
Due to transformer-based emotion and symbol analysis, the pipeline is GPU-intensive.

🆓 If you do not have a GPU, run on Google Colab using Free T4 GPU:

Open Colab

Upload the DreamProfiler.ipynb notebook

Go to Runtime > Change runtime type and select:

Hardware Accelerator: GPU

(T4 will be auto-selected)

🎯 Why No Traditional Accuracy Metrics?
Dream interpretation is inherently subjective and emotionally abstract. Therefore:

❌ BLEU, ROUGE, or F1 scores are not meaningful

✅ DreamProfiler uses clarity-based metrics like emotion entropy to compare internal emotional coherence

✅ User-specific profiling focuses on psychological continuity, not classification correctness

📊 Comparative Evaluation
Metric	DreamProfiler	DreamNet	Better
Emotion focus (entropy)	🔍 1.041 (lower)	🎲 1.734 (higher)	✅ DreamProfiler
Dominant emotion alignment	✅ Yes	❌ Weak	✅ DreamProfiler
Symbol breakdown	✅ Rich	❌ Vague	✅ DreamProfiler
Justification	✅ Provided	❌ None	✅ DreamProfiler
Charts clarity	✅ Structured	❌ Flat	✅ DreamProfiler

🔢 Why Emotion Entropy?
Emotion Entropy measures how focused or scattered the model's emotional interpretation is.

Lower entropy → One or few dominant emotions → emotionally precise

Higher entropy → Spread across emotions → emotionally ambiguous

DreamProfiler consistently exhibits lower entropy, indicating stronger emotional clarity in dream interpretation.

🧠 Key Modules
Emotion Analysis: Emotion detection using transformer models

Dream Embedding: User-specific memory via BERT-style embeddings

Dream Profiling: Extracts emotional patterns and top symbols

Comparative Visualization: Graph-based comparison across dreams/models

📂 Project Structure
bash
Copy
Edit
DreamProfiler/
├── dataset/                # Pre-downloaded dreams
├── DreamProfiler.ipynb     # Main pipeline notebook
├── utils/                  # Helper scripts (optional)
└── README.md               # Project documentation
🚀 Future Scope
Feedback-based interpretation refinement

Integration of cultural symbolism and dream motifs

Interactive web dashboard for dream history exploration

✅ Get Started
Load your dataset, start the notebook, and let DreamProfiler begin decoding the subconscious world — dream by dream.

vbnet
Copy
Edit

Let me know if you want this saved as `README.md` or auto-formatted into a downloadable PDF.
