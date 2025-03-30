# Mental Health Bot

A chatbot application that provides mental health information and support using LangChain and Hugging Face models.

## Features

- Uses Mistral-7B-Instruct-v0.3 model for generating responses
- Implements semantic search using FAISS vector store
- Streamlit-based web interface
- PDF document processing capabilities

## Setup

1. Clone the repository:
```bash
git clone https://github.com/singhalansh/mental-health-bot.git
cd mental-health-bot
```

2. Install dependencies using Pipenv:
```bash
pipenv install
```

3. Set up your environment variables:
Create a `.env` file in the root directory and add your Hugging Face API token:
```
HF_TOKEN=your_huggingface_token_here
```

4. Place your PDF documents in the `data/` directory

5. Run the document processing script:
```bash
python create_memo.py
```

6. Start the Streamlit application:
```bash
streamlit run medibot.py
```

## Project Structure

- `medibot.py`: Main Streamlit application
- `create_memo.py`: Script for processing PDF documents and creating vector store
- `connect_memo.py`: Module for connecting to the LLM and vector store
- `data/`: Directory for storing PDF documents
- `vectorstore/`: Directory containing the FAISS vector store

## Dependencies

- langchain
- faiss-cpu
- pypdf
- langchain-huggingface
- langchain-community
- streamlit

## License

MIT