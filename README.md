# RAG Based QA Assistant 

This project implements a document-based question-answering system using embeddings, vector storage, and natural language processing. It leverages models from Hugging Face for embeddings and inference, and uses ChromaDB for vector storage. The system ingests documents, stores them in a vector database, and provides a chat-based interface for querying information.

## Features

- **Data Ingestion**: Loads documents from a specified directory, processes them into vectors, and stores them in ChromaDB.
- **Vector Storage**: Uses ChromaDB to store and retrieve document vectors.
- **Question Answering**: Provides an interface to query the document database and retrieve relevant answers.
- **Hugging Face Models**: Utilizes Hugging Face models for text embeddings and inference.

 **Hugging Face Authentication:**

Ensure you have a Hugging Face token. You can obtain one by creating an account on [Hugging Face](https://huggingface.co/) and generating a token from the settings page.

## Configuration

Before running the script, update the following configurations in your script:

- **Hugging Face Token:**

    Replace `'YOUR_TOKEN'` with your actual Hugging Face token:

    ```python
    token='YOUR_TOKEN'
    ```

- **Directories and Paths:**

    - `KNOWLEDGE_BASE_DIR`: Directory where the documents are stored.
    - `CHROMA_DB_PATH`: Path to the ChromaDB database.

    Adjust these paths as needed based on your directory structure.




## Installation

To set up this project, follow these steps:

1. **Clone the Repository:**

    ```bash
    git clone <repository-url>
    cd <repository-directory>
    ```

2. **Create a Virtual Environment:**

    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows use `venv\Scripts\activate`
    ```

3. **Install Dependencies:**

    Install the required Python packages:

    ```bash
    pip install llama_index huggingface_hub chromadb
    ```
