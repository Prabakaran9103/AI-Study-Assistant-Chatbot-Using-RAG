# AI-Based Student Study Assistant Chatbot using Retrieval-Augmented Generation (RAG)

An AI-powered Study Assistant Chatbot that enables students to ask questions from multiple academic textbooks using **Retrieval-Augmented Generation (RAG)**. The application retrieves relevant information from uploaded PDF documents through semantic search and generates accurate, context-aware answers using the **Qwen2 Large Language Model**.

---

## Table of Contents

- Overview
- Features
- Technologies Used
- System Architecture
- Project Workflow
- Project Structure
- Installation
- Usage
- Example Workflow
- Learning Outcomes
- Future Enhancements
- Author

---

## Overview

Students often spend significant time searching through multiple textbooks to find relevant information. This project addresses that challenge by allowing users to upload academic PDF books and ask natural language questions. Instead of generating answers from general knowledge, the chatbot retrieves relevant content from the uploaded documents and uses it to produce accurate, context-aware responses.

The application is built using **Retrieval-Augmented Generation (RAG)**, which combines semantic document retrieval with the reasoning capabilities of a Large Language Model.

---

## Features

- Upload one or more academic PDF textbooks
- Automatic text extraction from PDF documents
- Intelligent text chunking for efficient retrieval
- Semantic search using FAISS vector database
- Context-aware question answering
- Interactive web interface built with Streamlit
- Responses generated only from uploaded study materials
- Easy-to-use interface for students

---

## Technologies Used

| Category | Technologies |
|----------|--------------|
| Programming Language | Python |
| Web Framework | Streamlit |
| RAG Framework | LangChain |
| Vector Database | FAISS |
| Embedding Model | Hugging Face Embeddings |
| Large Language Model | Qwen2 |
| PDF Processing | PyPDF |
| Machine Learning | Transformers, Torch |

---

## System Architecture

```
                     Academic PDF Books
                              │
                              ▼
                     Text Extraction
                              │
                              ▼
                      Text Chunking
                              │
                              ▼
                 Generate Text Embeddings
                              │
                              ▼
                 Store Embeddings in FAISS
                              │
                              ▼
                      User Question
                              │
                              ▼
                  Semantic Similarity Search
                              │
                              ▼
                 Retrieve Relevant Context
                              │
                              ▼
                 Qwen2 Large Language Model
                              │
                              ▼
                  Context-Aware Response
```

---

## Project Workflow

1. Upload one or more academic PDF textbooks.
2. Extract text from each uploaded document.
3. Split the extracted text into manageable chunks.
4. Generate embeddings for each chunk.
5. Store the embeddings in a FAISS vector database.
6. Convert the user's question into an embedding.
7. Retrieve the most relevant document chunks using semantic similarity.
8. Pass the retrieved context to the Qwen2 Large Language Model.
9. Display the generated answer through the Streamlit interface.

---

## Project Structure

```
AI-Study-Assistant-Chatbot-Using-RAG/
│
├── Source_Code/
│   ├── app.py
│   ├── app.bat
│   └── requirements.txt
│
├── Project_Report/
│   └── Project_Report.pdf
│
├── Presentation/
│   └── AI_Study_Assistant_Presentation.pptx
│
├── README.md
└── .gitignore
```

---

## Installation

### Clone the Repository

```bash
git clone https://github.com/Prabakaran9103/AI-Study-Assistant-Chatbot-Using-RAG.git
cd AI-Study-Assistant-Chatbot-Using-RAG
```

### Install Python

Download and install Python (3.12 or later):

https://www.python.org/downloads/

### Install Required Packages

```bash
pip install -r requirements.txt
```

### Run the Application

Using Command Prompt:

```bash
streamlit run app.py
```

Or simply run:

```
app.bat
```

---

## Usage

1. Launch the application.
2. Upload one or more academic PDF textbooks.
3. Wait until document processing is completed.
4. Enter a question related to the uploaded study materials.
5. View the generated answer based on the retrieved textbook content.

---

## Example Workflow

**Input Question**

```
What is the difference between process and thread?
```

**System Process**

- Search relevant textbook content
- Retrieve matching paragraphs
- Send retrieved context to Qwen2
- Generate the final answer

**Output**

A context-aware explanation generated using the uploaded textbooks.

---

## Learning Outcomes

Through this project, I gained practical experience in:

- Retrieval-Augmented Generation (RAG)
- Semantic Search
- Vector Databases (FAISS)
- Large Language Models
- Prompt Engineering
- LangChain
- Streamlit Application Development
- PDF Text Processing
- Information Retrieval

---

## Future Enhancements

- Chat history support
- User authentication
- Multiple LLM support
- Voice-based interaction
- OCR support for scanned PDFs
- Citation and source highlighting
- Cloud deployment
- Support for DOCX and PPTX documents
- Multi-user collaboration

---

## Author

**Prabakaran Chinnasamy**

M.Tech Computer Science and Engineering

Indian Institute of Technology Madras

GitHub: https://github.com/Prabakaran9103

---

## License

This project was developed for educational and academic purposes.
