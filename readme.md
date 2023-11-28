<!-- Readme for this project -->

# Candidate QnA - Gradio Application Powered by Google PaLM

This application provides a chat interface to a recruiter where they can upload a resume of a candidate and ask questions to the chat-bot about the candidate.

## The RAG process consists of three steps:

**Retrieval**: Relevant documents are retrieved from a knowledge base using a retrieval model.

**Augmentation**: The retrieved documents are used to augment the input text, providing the LLM with additional context.

**Generation**: The LLM generates text using the augmented input text.

In this project, Facebook AI Similarity Score is used to store and search vector embeddings, QA Retrieval Chain is used to retrieve and augment response and return to user. Application uses Gradio to provide a chat interface.

## How to start
1. Install requirements from pip install -r requirements.txt
2. Get a PaLM API key and create a .env file, store key in .env file like this `PaLM_API_KEY = <PaLM API Key>`
3. Start the gradio app using command - `gradio gradio_app.py`

## Demo

<img src="https://github.com/aadityasanjay0801/candidate-qna/blob/main/demo.gif" alt="Demo with a resume" width="3000" height="400">
<!-- https://github.com/aadityasanjay0801/candidate-qna/blob/main/demo.gif -->

