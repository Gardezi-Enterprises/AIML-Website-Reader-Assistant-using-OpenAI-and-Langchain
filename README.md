# AI-Based Applications for Natural Language Understanding and Information Extraction

This repository contains two AI-based application focused on natural language understanding and information extraction:


## 2. Website Reader Assistant using OpenAI and Langchain

### Overview
A Streamlit web application that allows users to input URLs of news articles and ask questions based on their content using OpenAI's GPT and Langchain tools.

### Technologies Used
- **Python**
- **Streamlit**: For interactive web UI.
- **Langchain**: For chaining language model components.
- **OpenAI**: LLM used for answering questions.
- **FAISS**: Vector database to store and retrieve article embeddings.
- **UnstructuredURLLoader**: Extracts content from provided URLs.
- **Environment Configuration**: Managed via `.env` and dotenv.

### How It Works
1. **URL Input**: User provides up to 3 news article URLs.
2. **Content Extraction**: Articles are loaded using `UnstructuredURLLoader`.
3. **Text Splitting**: Uses `RecursiveCharacterTextSplitter` for chunking.
4. **Embedding Generation**: Either OpenAI or HuggingFace embeddings.
5. **Vector Storage**: FAISS is used to store and index embeddings.
6. **QA Chain**: Langchain's `RetrievalQAWithSourcesChain` answers user questions based on the vector database.

### Requirements
- `streamlit`
- `openai`
- `langchain`
- `faiss-cpu`
- `python-dotenv`

---
