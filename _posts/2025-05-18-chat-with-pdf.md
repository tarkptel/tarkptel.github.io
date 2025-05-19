---
title: Chat with PDF Using Streamlit, LangChain & Hugging Face Transformers
date: 2025-05-19
tags: [AI, NLP, LangChain, Streamlit, PDF, Chatbot, HuggingFace, RAG]
---


I’m excited to share my latest project — **Chat with PDF** — a smart chatbot that allows you to upload any PDF document and chat with its content interactively!<br><br>

## What is Chat with PDF?

This project leverages the power of **Retrieval-Augmented Generation (RAG)** by combining:

- **Streamlit** — for building an easy and interactive web interface.
- **LangChain** — to create the document embeddings and handle query chaining.
- **Hugging Face Transformers** — for the underlying language model that answers your questions.

The best part? It runs completely without relying on OpenAI’s API, making it open-source and cost-effective.<br><br>

## Features

- Upload any PDF file and instantly chat with its contents.
- Extracts meaningful chunks and embeds them for quick retrieval.
- Interactive conversation window with context-aware answers.
- Lightweight and easy to deploy. <br><br>

## How It Works

1. The PDF is split into text chunks.
2. Each chunk is converted into vector embeddings.
3. When you ask a question, the relevant chunks are retrieved using similarity search.
4. The language model generates answers based on those chunks. <br><br>

## Why This Project?

With so many documents and reports stored as PDFs, it’s useful to interact with them conversationally instead of scrolling or searching manually.

This project is perfect for researchers, students, and anyone who wants quick insights from large PDF files. <br><br>

## Try It Out!

I’ve built this using Streamlit for easy deployment — check it out on [**Explore The App**](https://huggingface.co/spaces/tarkpatel/Chat_With_PDF) and give it a spin! <br><br>



**Technologies used:**

- Python
- Streamlit
- LangChain
- Hugging Face Transformers
- FAISS (for similarity search)

Feel free to reach out if you want to collaborate or have ideas to improve this project! <br><br>



*Thanks for reading!*


**Tark Patel**  
_Machine Learning Enthusiast & Developer_  
[LinkedIn](https://www.linkedin.com/in/tark-patel/) | [GitHub](https://github.com/tarkptel) <br><br>
