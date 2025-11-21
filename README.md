📘 # Multimodal & Multilingual RAG System

Author: Lakhan Bukkawar

This project implements a complete multimodal Retrieval-Augmented Generation (RAG) system with multilingual support.
It performs both image → text and text → image retrieval using a combination of CLIP, Multilingual CLIP, MarianMT translators, and FAISS vector search.

🚀 Key Features

🔍 Image → Text retrieval (8 languages)

🔁 Text → Image retrieval

🌍 Multilingual caption translation (MarianMT)

🧠 Embeddings using:

OpenAI CLIP ViT-B/32

Multilingual CLIP (50+ languages)

⚡ Efficient FAISS Search

HNSW index for image retrieval

FlatIP index for text retrieval

📊 Evaluation Metrics

Recall@K

Cosine Similarity

BERTScore

BLEU (optional)

🎨 t-SNE Visualization of Embeddings

🗂 Reproducible artifacts stored in submission_artifacts/

## 📂 Repository Structure

```
.
├── Multimodal_Multilingual_RAG_System.ipynb            # Main notebook (cleaned)
├── Multimodal_RAG_System_Report_LakhanBukkawar.pdf     # Technical report
├── Multimodal_RAG_Notebook_Export.pdf                  # PDF backup of notebook
├── Assignment - data science.pdf                       # Original assignment brief
│
├── clip-images-data/                                   # Dataset (8 images)
│   ├── camera.jpeg
│   ├── cat.jpeg
│   ├── coffee.jpeg
│   ├── girl.jpeg
│   ├── house_wife.jpeg
│   ├── motorcycle_right.jpeg
│   ├── page.png
│   ├── teacher.jpeg
│
└── submission_artifacts/                               # Generated outputs
    ├── faiss_index_images.faiss
    ├── image_embeddings.npy
    ├── final_translated_captions.csv
    ├── translated_captions_all8.csv
```




🔧 How to Run the Project

Clone or download this repository

Ensure the folders clip-images-data/ and submission_artifacts/ are in the same directory as the notebook

Open:
StockGro_GenAI_RAG_Assignment_LakhanBukkawar.ipynb

Run all cells from top to bottom

The system will:

Load images

Translate captions

Generate embeddings

Build FAISS indices

Perform multilingual retrieval

Compute evaluation metrics

Visualize embeddings using t-SNE

Save all artifacts automatically

🎯 Results Summary

100% Recall@K on CLIP-based image→text retrieval

Strong multilingual alignment across 8 languages

Cross-language consistency: all translated queries retrieve the same top image

Clear semantic structure in t-SNE visualization

All embeddings and FAISS indices stored for reproducibility

📄 Technical Report

Read the complete explanation of the methodology, results, and multilingual approach in:
📄 Multimodal_RAG_System_Report_LakhanBukkawar.pdf

🙌 Acknowledgements

This project uses open-source models from:

HuggingFace Transformers

SentenceTransformers

Facebook AI (FAISS)
