# StudyRAG — AI Document Assistant

StudyRAG is a private, locally-hosted AI study assistant that allows you to interact with your PDF documents using Retrieval Augmented Generation (RAG). It uses FastAPI for the backend, Vanilla JS for the frontend, and Ollama for local AI inference.

## 🚀 Key Features
- **Privacy First**: All documents and AI processing stay on your local machine.
- **Semantic Search**: Uses `nomic-embed-text` to find the most relevant parts of your PDFs.
- **Grounded Answers**: LLM responses are grounded in your uploaded documents to prevent hallucinations.
- **Modern UI**: Sleek, dark-themed responsive interface.

---

## 🛠️ Prerequisites

Before running the application, ensure you have the following installed:
1.  **Python 3.10+**
2.  **Ollama**: Download from [ollama.com](https://ollama.com/)

### Pull Required AI Models
Once Ollama is installed, run these commands in your terminal:
```bash
ollama pull llama3.2
ollama pull nomic-embed-text
```

---

## 📦 Installation

1.  **Clone the repository**:
    ```bash
    git clone https://github.com/Wtbaldw/StudyNotes-Rag-System.git
    cd StudyNotes-Rag-System
    ```

2.  **Create a Virtual Environment**:
    ```bash
    python -m venv .venv
    source .venv/bin/activate  # On Windows: .venv\Scripts\activate
    ```

3.  **Install Dependencies**:
    ```bash
    pip install -r requirements.txt
    ```

---

## 🏃‍♂️ Running the System

1.  **Start the Backend**:
    ```bash
    uvicorn main:app --reload
    ```

2.  **Open the Web Interface**:
    Navigate to `http://localhost:8000` in your web browser.

---

## 📄 Project Structure
- `main.py`: FastAPI backend, PDF parsing, and RAG logic.
- `public/`: Frontend assets (HTML, CSS, JavaScript).
- `uploads/`: Directory where processed PDFs are temporarily stored.
- `PROJECT_PROPOSAL.md`: Detailed technical project report.
- `WALKTHROUGH.md`: Summary of the development process.

---

## 📝 License
MIT License - Feel free to use this for your own study projects!