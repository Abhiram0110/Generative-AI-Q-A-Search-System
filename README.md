
# 💼 Finance and Accounting Q\&A Search System

This project is a domain-specific Question and Answer (Q\&A) system developed for **finance and accounting education**, built using **Generative AI** techniques. It leverages a **Retrieval-Augmented Generation (RAG)** architecture combining semantic search and large language models to help learners instantly access accurate answers from Kaplan Financial Education materials.

---

## 📚 Project Summary

Students and professionals preparing for finance certifications often face challenges finding specific information within massive, unstructured PDF materials. This project solves that problem by enabling natural language queries that retrieve contextually relevant answers using AI.

---

## 🎯 Business Objectives

* Help users locate relevant finance content without manual search.
* Improve study efficiency and knowledge retention.
* Deliver secure, accurate answers sourced directly from Kaplan’s content.
* Enable 24/7 access to finance education without instructor intervention.

---

## ⚙️ System Architecture

Our system uses a **Retrieval-Augmented Generation (RAG)** pipeline:

* **Storage**: Finance-related PDFs stored in Google Cloud Storage.
* **Embedding**: Hugging Face Sentence Transformers used for semantic embeddings.
* **Vector Search**: Vertex AI Matching Engine performs fast, scalable similarity search.
* **Language Model**: Gemini 2.5 Pro (via Vertex AI) generates final natural language answers.
* **Framework**: LangChain’s `RetrievalQA` coordinates retrieval and response generation.
* **Environment**: Developed and tested using Google Colab.

---

## 🛠️ Key Technologies

| Component            | Technology Used                      |
| -------------------- | ------------------------------------ |
| Cloud Platform       | Google Cloud Platform (GCP)          |
| Programming Language | Python                               |
| Embeddings           | Sentence Transformers (Hugging Face) |
| Vector Store         | Vertex AI Matching Engine            |
| LLM                  | Gemini 2.5 Pro                       |
| Framework            | LangChain                            |
| Notebook Environment | Google Colab                         |

---

## 📈 Implementation Phases

1. **Data Collection**: 100+ finance/accounting PDFs curated and stored in GCP.
2. **Text Processing**: PDFs parsed and chunked into retrievable units.
3. **Embedding & Indexing**: Semantic vectors stored in Vertex Matching Engine.
4. **Query Handling**: LangChain pipeline finds top relevant chunks.
5. **Answer Generation**: Gemini 2.5 Pro produces grounded, fluent responses.
6. **System Testing**: 10 diverse finance prompts tested for reliability and accuracy.

---

## 🔎 Sample Questions Handled

* What is the purpose of an income statement?
* What is the difference between share capital and retained earnings?
* Why is balancing your checking account important?
* What led to the emergence of Eurocurrency markets during the Cold War?
* Define the concept of ‘Future Value’ in finance.

The system gracefully declines unrelated prompts (e.g., science questions like “What is displacement?”), demonstrating responsible output filtering.

---

## 🧪 Evaluation Results

The system consistently delivered correct, contextual responses for in-domain questions. For example, complex concepts like FICO scores, offshore banking pros/cons, and accounting standards were handled accurately and fluently.

---

## 📁 Repository Structure

* `Team4_5770_project_NEW.ipynb`: Main development notebook.
* `Data.zip`: Educational PDFs used for semantic retrieval.
* `ADTA_5770_SEMESTER_PROJECT_submission_prompts_responses_group4.docx`: Prompt-response evaluations.
* `FINAL REPORT.docx`: Full system design, implementation, and analysis.

---



