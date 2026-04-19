RAG Agent with LangGraph
Overview

This project implements a Retrieval-Augmented Generation (RAG) Agent using LangChain and related tools. The notebook demonstrates how to load documents (PDFs), process them into embeddings, store them in a vector database, and query them using a language model.

Features
Load and process PDF documents
Split text into manageable chunks
Generate embeddings using Hugging Face models
Store embeddings in a vector store
Build a retrieval-based question-answering system
Use an agent-based workflow with tools
Tech Stack
Python
LangChain
LangGraph
Hugging Face Embeddings
Ollama (LLM interface)
Pydantic
Key Components
Document Loader: Loads PDF files using PyPDFLoader
Text Splitter: Splits documents into chunks using RecursiveCharacterTextSplitter
Embeddings: Converts text into vector representations
Vector Store: Stores embeddings for similarity search
LLM: Uses Ollama-based chat model
Agent Graph: Built using LangGraph for structured workflows
Installation

Install required dependencies:

pip install langchain langgraph langchain-community langchain-core \
langchain-text-splitters langchain-huggingface langchain-ollama \
pydantic
Usage

Open the notebook:

jupyter notebook "RAG AGENT.ipynb"
Update the PDF file path in the notebook
Run all cells step by step:
Load document
Split text
Create embeddings
Store in vector DB
Query using the agent
Example Workflow
Load PDF
Split into chunks
Generate embeddings
Store in vector database
Ask questions → Retrieve relevant chunks → Generate answer
Notes
Ensure Ollama is running locally if used as the LLM backend
Large PDFs may require optimization (chunk size, overlap)
Clear outputs before committing to GitHub for smaller file size
Future Improvements
Add support for multiple documents
Integrate different vector databases (FAISS, Chroma)
Improve agent decision-making
Add UI (Streamlit or Gradio)
License

This project is open-source and free to use.
