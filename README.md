# Hotel Booking Analytics with LLMs

This project integrates a Language Model to interpret natural language hotel booking queries and generate meaningful analytics using ChromaDB and Flask.

## Features
- LLM-powered query understanding (intent + filters).
- Vector-based document search with SentenceTransformers and ChromaDB.
- Flask API for answering questions and generating analytics.
- Easy to run and extend.

## Setup Instructions

### 1. Clone the repo
```bash
git clone https://github.com/your-username/llm-hotel-analytics.git
cd llm-hotel-analytics
```

### 2. Install dependencies
```bash
pip install -r requirements.txt
```

### 3. Start the app
```bash
python app.py
```

Flask will start on `http://localhost:5000`.

## API Usage

### `POST /ask`
```json
{
  "question": "What is the average price of a hotel booking in Portugal in July 2017?"
}
```

### `POST /analytics`
Returns analytics about stored bookings in vector DB.

---

**Authors:** You  
**Tech Stack:** Python, Flask, HuggingFace Transformers, SentenceTransformers, ChromaDB