# RAG-Based Corporate Knowledge Bot

## Description

This project is an intelligent "Smart-Policy" Q&A bot. It uses a **Retrieval-Augmented Generation (RAG)** pipeline to answer questions based *only* on a set of internal company documents.

This approach prevents the LLM from hallucinating and ensures all answers are factually grounded in the provided knowledge base.

## Tech Stack

* **Python**
* **LangChain**
* **OpenAI API** (for LLM reasoning)
* **Hugging Face** (for local embeddings)
* **FAISS** (for vector storage)

## Setup & Installation

1.  Clone the repository:
    ```bash
    git clone [your-repo-link]
    cd [your-repo-name]
    ```

2.  Install the required Python libraries:
    ```bash
    pip install langchain-openai langchain-huggingface langchain_community faiss-cpu tiktoken langchain-text-splitters langchain
    ```

3.  Set up your environment variable. You can do this by creating a `.env` file and adding your API key:
    ```
    OPENAI_API_KEY="sk-your-secret-key-here"
    ```

4.  Add your knowledge base documents (e.g., `policy.txt`) to the root directory.

## Usage

Run the main application script from your terminal:

```bash
python app.py
