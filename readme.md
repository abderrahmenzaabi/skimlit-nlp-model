# 🧠 PubMed Abstract Sentence Classification

A deep learning project for classifying individual sentences in scientific abstracts into their role (e.g., Background, Methods, Results, etc.) using the [PubMed 200k RCT dataset](https://github.com/Franck-Dernoncourt/pubmed-rct).  

This notebook implements a **hybrid deep learning model** combining:
- **Token-level embeddings** using the Universal Sentence Encoder (USE),
- **Character-level embeddings** with BiLSTM,
- **Positional embeddings** using line numbers and total lines in abstracts.

---

## 📂 Dataset

We use the **PubMed 200k RCT** dataset, which contains 200,000 structured abstracts from PubMed.

Each sentence is annotated with one of five labels:
- `BACKGROUND`
- `OBJECTIVE`
- `METHODS`
- `RESULTS`
- `CONCLUSIONS`