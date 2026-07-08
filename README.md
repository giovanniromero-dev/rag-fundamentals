# RAG Course

Course workspace for learning and experimenting with Retrieval-Augmented
Generation (RAG). The repository currently contains the initial Python setup and
the first data ingestion and parsing notebook.

## Current Contents

- `0-DataIngestParsing/1-dataingestion.ipynb`: introductory notebook for the
  data ingestion and parsing module.
- `main.py`: minimal Python entry point for the project.
- `pyproject.toml`: Python project metadata and pinned runtime requirement.
- `uv.lock`: locked dependency graph for reproducible installs with `uv`.
- `requirements.txt`: pip-compatible dependency list.
- `.python-version`: local Python version pin.

## Requirements

- Python 3.13 or newer
- `uv` for the lockfile-based setup, or `pip` with `requirements.txt`
- A local `.env` file for API keys when provider integrations are used

The `.env` file is intentionally ignored by Git.

## Setup

Using `uv`:

```bash
uv sync
```

Using `pip`:

```bash
python -m venv .venv
.venv\Scripts\activate
pip install -r requirements.txt
```

## Run

```bash
python main.py
```

Expected output:

```text
Hello from rag-course!
```

## Main Dependencies

- LangChain and LangChain community integrations
- LangChain OpenAI and Groq integrations
- ChromaDB and FAISS for vector storage/search experiments
- Sentence Transformers for embeddings
- PyPDF for PDF parsing
- TikToken for tokenization utilities
- python-dotenv for local environment loading
- IPython kernel support for notebooks
