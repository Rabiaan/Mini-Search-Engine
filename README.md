# Mini Search Engine

A Streamlit app that lets you upload PDFs, index them into Pinecone vector database, and search using natural language queries.

## Features

- Upload PDF documents (minimum 5 required)
- Extract text and embed using sentence-transformers (`all-MiniLM-L6-v2`)
- Store embeddings in Pinecone vector database
- Semantic similarity search with natural language queries

## Setup

1. Install dependencies:
   ```
   pip install -r requirements.txt
   ```

2. Create `.env` file with your Pinecone API key:
   ```
   PINECONE_API_KEY=your_api_key_here
   ```

3. Run the app:
   ```
   streamlit run app.py
   ```

## Requirements

- streamlit
- sentence-transformers
- PyMuPDF
- pinecone-client
- python-dotenv
- torch