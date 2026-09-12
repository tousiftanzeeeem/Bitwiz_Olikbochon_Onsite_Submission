# 🏆 Bitwiz — অলীকবচন (Olikbochon)

### **Most Novel Approach Award Winner**  
**IUT 12th ICT Fest Datathon 2026**  
*Bengali LLM Hallucination Detection Challenge*

---

<div align="center">

![Award](https://img.shields.io/badge/Award-Most%20Novel%20Approach-gold?style=for-the-badge)
![Event](https://img.shields.io/badge/Event-IUT%2012th%20ICT%20Fest-blue?style=for-the-badge)
![Theme](https://img.shields.io/badge/Theme-অলীকবচন-purple?style=for-the-badge)
![Language](https://img.shields.io/badge/Language-Bengali-green?style=for-the-badge)

</div>

---

## 🧠 Overview

**Bitwiz** is our solution to the **অলীকবচন (Olikbochon)** challenge — a specialized competition focused on detecting hallucinations in Large Language Model outputs for the Bengali language.

Our system combines:

- **Deterministic Cascade Classification**
- **Category-gated Retrieval-Augmented Generation (RAG)**
- **Specialized handling** for Math, Lexical, General Knowledge, and Relation (synonym/antonym) queries
- **Offline-first architecture** optimized for Kaggle/competition constraints

We were awarded **Most Novel Approach** for the creativity and effectiveness of our multi-stage, category-aware pipeline.

---

## ✨ Key Highlights of Our Approach

| Component                  | Description                                                                 |
|---------------------------|-----------------------------------------------------------------------------|
| **Cascade Classifier**    | Deterministically routes questions into Math, Bangla-only, Null GK, and Non-null GK buckets |
| **Category-Gated RAG**    | Only retrieves external knowledge when truly needed (skips Math & pure lexical cases) |
| **Relation Strategy**     | Specialized retrieval path for synonym / antonym questions                  |
| **Lexical Archive**       | Curated Bangla idioms & meanings integration                                |
| **Offline Stack**         | Fully offline inference using quantized Qwen3 + BGE-M3 + reranker           |

---


## 👥 Team Bitwiz

| Member                    | GitHub                                     
|---------------------------|---------------------------------------------
| **Tanzim Tousif**         | [tousiftanzeeeem](https://github.com/tousiftanzeeeem) 
| **Mohammed Afham Adian**  | [AfhamAdian](https://github.com/AfhamAdian)         
| **Suprio Paul**           | [Suprio85](https://github.com/Suprio85)             
| **Sijon Chisty Saon**     | [Saon110](https://github.com/Saon110)               

All members are undergraduate students from the **Department of Computer Science and Engineering, Bangladesh University of Engineering and Technology (BUET)**.

---

## 🛠️ Tech Stack

- **LLM**: Qwen3-5-35B-A3B (GPTQ INT4)
- **Embeddings**: BGE-M3
- **Reranker**: BAAI BGE Reranker v2-M3
- **Vector Store**: FAISS
- **Inference**: vLLM (offline wheels)
- **Language**: Python + Jupyter
- **Environment**: Fully offline Kaggle-compatible pipeline

---

## 🚀 How to Run

1. Open `Bitwiz_inference_notebook.ipynb` on Kaggle (or locally with the required datasets attached).
2. Update only the path variables in the first cell if needed.
3. Run all cells sequentially.

The notebook is designed to be self-contained and competition-ready.

---

## 📜 Documents

- 📄 **[Technical Report](Bitwiz_report.pdf)** — Full methodology, experiments, and analysis  
- 📊 **[Presentation Slides](Bitwiz_presentation.pdf)** — Onsite defense presentation  

---

## 🏅 Acknowledgement

We are deeply grateful to the organizers of **IUT 12th ICT Fest** and **Brain Lab (EBLICT Project)** for creating such a meaningful and challenging problem around **Bengali LLM reliability**.

Special thanks to the judges for recognizing the novelty of our category-aware, hybrid deterministic + retrieval approach.

---

<div align="center">

**Built with ❤️ by Team Bitwiz**  
*BUET CSE*

</div>
