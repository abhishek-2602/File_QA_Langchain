# File_QA_Langchain


## Overview
This notebook demonstrates how to implement a file-based question-answering system using LangChain and open-source large language models (LLMs). The system allows users to query documents and receive context-aware answers. The workflow includes:
- Uploading and processing documents (PDF, text, CSV, etc.)
- Splitting text into chunks
- Creating embeddings
- Storing embeddings in a vector database
- Querying the document using natural language
- Returning context-specific answers from the model

## Requirements
The following Python libraries are required:
- langchain
- openai
- tiktoken
- chromadb
- faiss-cpu
- sentence-transformers
- transformers (if using Hugging Face models)
- huggingface_hub (if accessing Hugging Face-hosted models)

Install them using:
```bash
pip install langchain openai tiktoken chromadb faiss-cpu sentence-transformers transformers huggingface_hub
```

## Usage
1. Launch Jupyter Notebook:
```bash
jupyter notebook FileQA_opensourcemodel_langchain_day_2.ipynb
```
2. Upload a file (such as a PDF or TXT) when prompted or set the file path in the notebook.
3. The notebook will:
   - Load and parse the document
   - Generate embeddings
   - Store embeddings in the vector database
   - Allow question answering via natural language queries
4. Run the cells sequentially to build and test the Q&A pipeline.

## Output
The notebook provides:
- Logs of embedding creation and vector storage
- Retrieval results from the vector database
- Natural language answers to user queries

## Notes
- The default configuration may rely on open-source Hugging Face models. Ensure the correct model name and API tokens (if required) are specified.
- The workflow can be extended into a production-ready application using frameworks such as Streamlit or FastAPI.
- You can experiment with different vector stores (Chroma, FAISS, Weaviate) depending on performance and scalability requirements.
