# Chat with Your Data Bot

A Python-based chatbot that allows you to have interactive conversations with your PDF documents using LangChain and GPT models.

## Features

- Upload and process PDF documents
- Interactive chat interface with your documents
- View chat history and database queries
- Clear conversation history
- Real-time responses using GPT-3.5-turbo (or GPT-4)
- Source tracking for answers

## Prerequisites

- Python 3.7+
- OpenAI API key

## Installation

1. Clone the repository
2. Install the required packages:
```bash
pip install -r requirements.txt
```
3. Copy `.env.example` to `.env` and add your OpenAI API key
4. Run the application:
```bash
python chat_with_pdf.py
```

## Usage

1. Open the application in your web browser
2. Navigate to the 'Configure' tab to upload a PDF file
3. Click 'Load DB' to process the document
4. Switch to the 'Conversation' tab to start chatting
5. View source documents and database queries in the 'Database' tab
6. Check your chat history in the 'Chat History' tab

## Project Structure

- `chat_with_pdf.py`: Main application file
- `requirements.txt`: Python dependencies
- `.env`: Environment variables (API keys)

## Notes

- The default model is set to "gpt-3.5-turbo", but you can change it to "gpt-4" if you have access
- Documents are processed in chunks of 1000 characters with 150 character overlap
- The application uses in-memory vector storage (DocArrayInMemorySearch)