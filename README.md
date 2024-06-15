# Building an End-to-End RAG Application with GPT-4o and ObjectBox
![image](https://github.com/GayaaniD/RAG-Application-with-GPT-4o-ObjectBox/assets/125920863/9fdbe83b-b377-49db-baa2-8686fc9365ee)

This project is about building an end-to-end Retrieval-Augmented Generation (RAG) application that leverages the power of GPT-4o alongside ObjectBox, an open-source vector database. This combination allows us to efficiently store and retrieve information while enabling GPT-4o to answer your questions in a conversational manner.

## Project Flow
### 1. Data Loading and Preprocessing:
  - Fetch the content from a target website (e.g., LangSmith user guide) using LangChain’s document loaders.
  - The retrieved text will be split into smaller chunks for efficient processing.
### 2. Vectorization:
  - Each text chunk is converted into a mathematical representation (vector) using LangChain’s integration with OpenAI embeddings and store it in ObjectBox vector database.
  - This vector database serves as the foundation for information retrieval within the RAG system.
### 3. Building the RAG Pipeline:
  - Leverage LangChain’s pre-built RAG prompt from Hugging Face to structure our prompts for GPT-4o.
  - The retrieved vectors act as an internal search engine, enabling GPT-4o to find the most relevant information for answering your questions.
### 4. User Interaction:
  - Interact with the RAG application by posing questions in a chat-like interface.
  - Retriever will the most relevant passages from vector database, and GPT-4o use them to formulate a response based on the pre-defined RAG prompt.

**Takes user question as input and utilizes the qa_chain. Utilize the vector database to retrieve the most relevant information (text chunks) based on the question. Use the pre-built RAG prompt to structure the retrieved information and the user question for GPT-4o to process. Generate a response (answer) based on the processed information.**

