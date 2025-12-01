# QuizLit

QuizLit is an AI-driven quiz generation platform that converts documents into structured, multi-format quizzes using LLMs. It supports difficulty levels, multi-format questions, PDF export, and a clean API + UI layer built for scale.


## Overview
QuizLit transforms learning materials into interactive quizzes using advanced NLP pipelines:

- Upload documents → system ingests + chunks text
- Embeds content using vector embeddings
- Stores in ChromaDB
- Retrieves context using similarity search
- LLM generates high-quality questions
- Additional quality-enhancement stage improves formatting + correctness
- Quizzes can be taken, exported, or integrated via API



## ✨ Features
###🔹 Core AI Pipeline 
- Document Ingestion: Supports PDFs, text files, and lecture notes
- Text Chunking: Intelligent chunking for optimized retrieval
- Embedding Generation: Uses sentence transformers/LLM embeddings
- ChromaDB Vector Storage: Fast, persistent similarity lookup
- Retrieval Pipeline: Converts user prompts → context-aware inputs
- LLM Question Generation: Auto-creates questions from context
- Basic Quiz Logic: Initial formatting + question structuring
### Upcoming
- ✔ Difficulty levels
- ✔ Multiple quiz formats (MCQ, True/False, Fill-in-the-blank)
- ✔ Quality enhancement stage (grammar + clarity + distractor validation)
- ✔ PDF export for quizzes
- ✔ FastAPI backend
- ✔ React frontend
- ✔ Error handling + validation
- ✔ Docker support for full stack

---

## 🛠 Tech Stack

| Component | Technology | Description |
| :--- | :--- | :--- |
| **Backend** | Python, FastAPI | Core API layer, quiz logic, routing |
| **AI Pipeline** | LangChain, LLMs, Sentence-Transformers | Embeddings, retrieval, and question generation |
| **Vector DB** | ChromaDB | Stores document embeddings and enables semantic search |
| **Frontend** | React + Vite, TypeScript | Fast and modern UI framework |
| **Styling** | TailwindCSS | Utility-first CSS for rapid UI styling |
| **Export Engine** | ReportLab / pdfkit | PDF quiz generation |
| **Containerization** | Docker, Docker Compose | Production-ready environment setup |
| **Build Tools** | Node.js, npm / yarn | Needed for frontend development |

---

## 📁 Project Structure

- **QuizLit/**
  - **backend/** 
  - **frontend/**
  - `docker-compose.yml`
  - `README.md`

---

## Installation

### Prerequisites
Before you begin, ensure you have the following installed on your system:
- Python 3.6 or higher
- Node.js 18 or higher
- Docker & Docker Compose (optional but recommended)

### Step-by-Step Installation Guide

1. **Clone the Repository**
   
   Start by cloning the repository to your local machine. Use the following command:
   ```bash
   git clone https://github.com/your-username/QuizLit.git
   cd QuizLit

--- 

## Set Up a Virtual Environment (Optional but recommended)

It's a good practice to create a virtual environment for your Python projects. This keeps your project dependencies isolated. If you have `virtualenv` installed, create a new environment with:

```bash
virtualenv venv
source venv/bin/activate
```

## Install Dependencies
Inside the virtual environment, install all necessary dependencies by running:
```bash
pip install -r requirements.txt
```

---

## 📝 License

MIT License — free to use, modify, and distribute.
