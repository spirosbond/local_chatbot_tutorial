# Langchain Local Chatbot Tutorial

This tutorial guides you through the process of running an interactive chatbot locally using Langchain. The primary focus is on Retrieval Augmented Generation (RAG), where a Language Model (LLM) retrieves contextual documents from an external dataset as part of its execution.

**Notebook Link:** [My Local Chatbot](my_local_chatbot.ipynb)

## Overview
This tutorial is inspired by the ["LangChain Chat with your data"](https://learn.deeplearning.ai/langchain-chat-with-your-data/lesson/1/introduction) course at Deeplearning.ai. We will heavily rely on Langchain and its libraries to achieve retrieval augmented generation. The models and generated vectors are stored and run locally. 

**Disclaimer:** While all models and files remain local, data leaks are not guaranteed, and the author is not responsible for any issues. Avoid using sensitive or classified information.

## Dependencies
Dependencies will be installed as we progress. The notebook was tested under WSL2; results may vary on other platforms. The tutorial is adaptable to run on CPU for users without GPU.

## Document Loading
The tutorial begins with loading documents from PDFs, YouTube video transcripts, and URLs. The necessary libraries and dependencies are installed in this section.

## Document Splitting
Documents are split into chunks using a text splitter, essential for creating embeddings later in the tutorial.

## Creating Vector scores and Embeddings
Vector scores and embeddings are generated using the BGE-small model from Hugging Face. The embeddings are stored in a local Chromadb.

## Retrieval Techniques
Various retrieval techniques, including similarity search, max marginal relevance search, and similarity score search, are demonstrated. These techniques help find relevant information based on a user's question.

## Retrieval via LLMs (Compression)
A compression retriever using the Mistral Instruct model is introduced. This retriever compresses documents retrieved by similarity score search.

## Q&A
The final section involves asking questions to the model. A chat chain is set up to maintain chat history and context, enabling more context-aware responses.

Please follow the notebook step-by-step to set up and run your local Langchain-based chatbot.

## Useful links
- https://python.langchain.com/docs/get_started/introduction
- https://github.com/ggerganov/llama.cpp?tab=readme-ov-file
- https://github.com/imartinez/privateGPT
- https://www.trychroma.com/
- https://stackoverflow.com/questions/28908319/how-to-clear-jupyter-notebooks-output-in-all-cells-from-the-linux-terminal
- https://learn.deeplearning.ai/langchain-chat-with-your-data/lesson/1/introduction