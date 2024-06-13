# Retrieval Augmented Generation(RAG) with LlamaIndex
This project is a Streamlit web application that allows users to ask questions about the contents of a set of documents. It leverages OpenAI's GPT-3.5-turbo model for natural language processing and the llama_index library for indexing and querying document contents.

## Features

The chatbot employs a Retrieval-Augmented Generation (RAG) pipeline, which involves the following steps:

1. **Document Loading**: Documents are loaded from a specified directory and processed.
2. **Indexing**: The contents of the documents are indexed. This step creates a searchable index that maps relevant sections of the documents to key terms and phrases.
3. **Retrieval**: When a user asks a question, the query is first used to retrieve relevant document sections from the index.
4. **Generation**: The retrieved document sections are then passed to the OpenAI GPT-3.5-turbo model, which generates a context-aware response based on the retrieved information.

## Architecture

The "llama_index" library is central to building this chatbot, providing the necessary tools for indexing and querying document contents. LlamaIndex is a framework that allows us to ingest custom content/data and allows us to query that content. The following picture shows a high level approach of how LlamaIndex works :
![image](https://github.com/subhanjan160901/nutrition_llm/assets/55011614/10bef7a6-7522-4c83-b9f3-de4d2a5d7541)
