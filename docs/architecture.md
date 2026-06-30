# System Architecture

## High-Level Overview

The Maximo AI Incident Investigator is a Retrieval-Augmented Generation (RAG) application that helps enterprise support teams troubleshoot IBM Maximo incidents using AI.

## Components

### 1. User Interface
- Streamlit Web Application
- Upload documents
- Ask questions
- View incident summaries

### 2. Document Processing
Supported file types:
- PDF
- DOCX
- TXT
- XML
- LOG

The application extracts text from uploaded files.

### 3. Chunking

Large documents are split into smaller chunks.

Purpose:
- Better retrieval
- Faster search
- Higher answer quality

### 4. Embedding Model

Each chunk is converted into a numerical vector (embedding).

Purpose:
Allow semantic search instead of keyword search.

### 5. Vector Database

Stores embeddings.

Examples:
- ChromaDB
- FAISS

Purpose:
Retrieve the most relevant document chunks.

### 6. Large Language Model

The retrieved context is sent to an LLM.

The LLM generates:
- Root cause
- Recommendations
- Incident summaries
- Answers with citations

## Workflow

User uploads documents

↓

Text Extraction

↓

Chunking

↓

Embeddings

↓

Vector Database

↓

User asks question

↓

Semantic Search

↓

LLM

↓

Answer with citations
