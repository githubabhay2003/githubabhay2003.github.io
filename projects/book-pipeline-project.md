# Project: Automated Book Publication Workflow

An advanced, AI-driven pipeline that automates the entire book publishing workflow, from web-based chapter extraction to AI-powered rewriting, human-in-the-loop review, and semantic versioning in a vector database.

[Back to Home](./index.md)

---

### 1. The Goal
The objective was to architect a robust, automated pipeline that leverages modern AI to streamline the book publication process. The system is designed to fetch raw chapter text from a web source, use a Large Language Model (FLAN-T5) for rewriting ("spinning"), facilitate a human review phase, evaluate edits with RL-based metrics, synthesize the final text into audio, and meticulously version each iteration using a vector database for semantic search.

---

### 2. My Role & Contributions
As the sole architect and engineer, I designed and built this complex, multi-stage system from the ground up, integrating various AI and data technologies into a cohesive workflow.

* **AI Pipeline Orchestration:** I developed the master script that controls the flow of data through each stage: scraping, AI writing, human editing, scoring, voice synthesis, and versioning.
* **LLM Integration:** I implemented the Google FLAN-T5 model using the `transformers` library to perform the core text generation and rewriting tasks.
* **Human-in-the-Loop & RL Metrics:** I designed the human review module and implemented a reward system based on NLP metrics (BLEU score, Flesch Reading Ease) to objectively measure the quality of human edits.
* **Vector Database & Versioning:** I used ChromaDB to create a sophisticated version control system. Each version of the chapter is not just stored, but "embedded" as a vector, enabling powerful semantic search to find previous revisions based on meaning, not just keywords.
* **Component Development:** I wrote all the individual Python modules for web scraping (Playwright), voice synthesis (`pyttsx3`), and interacting with the ChromaDB vector store.

---

### 3. Technologies Used
* **AI & Machine Learning:** FLAN-T5 (LLM), PyTorch, `transformers`, Reinforcement Learning Concepts (`nltk`, `textstat`).
* **Data & Vector DB:** ChromaDB, `sentence-transformers`.
* **Web Automation:** Playwright.
* **Voice Synthesis:** `pyttsx3`.
* **Core Language:** Python.

---

### 4. Project Links
* **[View Code & Pipeline on GitHub](https://github.com/githubabhay2003/Automated-Book-Publication-Workflow)**

---
