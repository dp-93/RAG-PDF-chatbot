# RAG-PDF-chatbot
# 💬 Chat with Your PDF: A Custom Knowledge Chatbot

This is an advanced AI application that allows you to have a conversation with your own documents. By uploading a PDF, you can ask questions and receive answers based *only* on the content of that document. This project is a practical implementation of **Retrieval-Augmented Generation (RAG)**, the state-of-the-art technique for building chatbots with custom knowledge bases.

![Demo GIF of the Chat with PDF App](link_to_your_gif.gif)

## How It Works

The application follows the complete RAG pipeline:
1.  **Document Loading & Processing:** When a user uploads a PDF, the system reads the text and splits it into smaller, manageable chunks.
2.  **Vector Embeddings:** Each chunk of text is converted into a numerical representation (an embedding) using Google's powerful embedding models.
3.  **Knowledge Base Creation:** The embeddings are stored in a `FAISS` vector database, creating a searchable index of the document's content.
4.  **Retrieval & Generation:** When a user asks a question, the system finds the most relevant chunks from the database and feeds them to Google's Gemini model along with the original question, ensuring the answers are accurate and grounded in the provided context.

## Technologies Used

-   **AI & Machine Learning:**
    -   `LangChain`: The core framework for building the RAG pipeline.
    -   `Google Gemini API`: Used for the generative language model and embeddings.
    -   `FAISS`: For creating the efficient in-memory vector database.
-   **Application & Deployment:**
    -   `Gradio`: To build and deploy the interactive web application.
    -   `Python`: The primary programming language.
    -   `PyPDF2`: For extracting text from PDF documents.

## Key Skills Demonstrated

-   **Retrieval-Augmented Generation (RAG):** Full implementation of an advanced AI system.
-   **Large Language Model (LLM) Integration:** Using powerful models like Gemini via APIs.
-   **Vector Databases & Embeddings:** A deep understanding of how to create and query a knowledge base.
-   **Interactive Application Development:** Building a user-friendly, step-by-step interface with Gradio.
-   **Advanced Debugging:** Solved complex environment and library compatibility issues.
