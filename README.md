# Side Project: RAG with Langchain using [VinaLlama-2](https://huggingface.co/vilm/vinallama-2.7b-chat) (chat model)

## Introduction
This project focuses on applying RAG to improve the accuracy of answers from LLMs, specifically VinaLlama-2. The workflow includes steps such as loading the model, creating a pipeline for generating answers, splitting the document, creating a processing chain with prompts, and using reranking techniques to improve the accuracy of the results.

## Main Goals
The main goal of the project is to create a system that is capable of:

1.Loading and using LLMs available on Huggingface.
2.Processing and extracting text from documents in various formats (PDF, Markdown, etc.).
3.Generating embeddings from documents and using them to perform semantic search.
4.Applying reranking techniques to optimize search results, ensuring the most relevant results to the query.
5.Using processing chains to integrate multiple steps into a seamless process.

## Main Components
- **Load Model**: Loads the language model and tokenizer from the `transformers` library.
- **Transformers Pipeline**: Creates a pipeline to generate text automatically based on the downloaded model.
- **Prompt Template**: Builds standard prompt templates to provide input to the model.
- **Document Loader**: Loads and processes multiple types of document files from multiple sources, including local or linked.
- **Document Splitter**: Splits large documents or documents into smaller parts for easier processing.
- **Embedding**: Creates vector embeddings from text segments to perform semantic search.
- **Embedding Database**: Stores and retrieves embeddings for searching and matching.
- **Reranking**: Reranking techniques are applied to reorder search results by relevance.
- **Chain Workflow**: Create processing chains with multiple linked steps, from document loading, text generation, to semantic search and reranking.
