# LLM_RAG_Contract-Advisor_App

![image](https://github.com/Diriba1/LLM_RAG_Contract-Advisor_App/assets/39425889/98d9e3d8-cb7f-4747-b7df-e598c7d95809)


Build, Evaluate, and Improve the RAG system for Contract Q&A (chatting with a contract and asking questions about the contract).

This Chat App is a Python application that allows you to chat with contract documents. You can ask questions about the contracts, and the application will provide relevant responses based on the content of the contracts you provide. This app utilizes a language model to generate accurate answers to your queries. Please note that the app will only respond to questions related to the loaded PDFs.

### How It Works
The application follows these steps to provide responses to your questions:

- PDF Loading: The app reads multiple PDF documents and extracts their text content.

- Text Chunking: The extracted text is divided into smaller chunks that can be processed effectively.

- Language Model: The application utilizes a language model to generate vector representations (embeddings) of the text chunks.

- Similarity Matching: When you ask a question, the app compares it with the text chunks and identifies the most semantically similar ones.

- Response Generation: The selected chunks are passed to the language model, which generates a response based on the relevant content of the PDFs.
  
### Dependencies and Installation
To install please follow these steps:

Clone the repository to your local machine.

```git clone https://github.com/Diriba1/LLM_RAG_Langchain_Contract-Advisor_App/```

Install the required dependencies by running the following command:

```pip install -r requirements.txt```

Obtain an API key from OpenAI and Huggingface and add it to the .env file in the project directory.

`OPENAI_API_KEY=your_secret_api_key`

`HUGGINGFACEHUB_API_TOKEN=your_secret_api_key`

### Usage
Ensure that you have installed the required dependencies and added the OpenAI API or HuggingFace key to the .env file.

Run the app.py file using the Streamlit CLI. Execute the following command:

```streamlit run app.py```

The application will launch in your default web browser, displaying the user interface.

Load your contract PDF documents into the app by following the provided instructions.

Ask questions about the loaded contract PDFs using the chat interface.
