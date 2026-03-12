RAG Gemini PDF Chat (Spring Boot + Gemini + PostgreSQL)

An AI-powered PDF Question Answering System built using RAG (Retrieval-Augmented Generation).

Users can upload a PDF and ask questions about the document.
The system retrieves relevant chunks using vector similarity search and generates answers using Google Gemini AI.

⸻

Tech Stack
	•	Java 17
	•	Spring Boot
	•	PostgreSQL + pgvector
	•	Google Gemini API
	•	Apache PDFBox
	•	REST APIs

⸻

Features
	•	Upload PDF documents
	•	Automatically split text into chunks
	•	Generate embeddings using Gemini
	•	Store embeddings in PostgreSQL vector database
	•	Perform similarity search
	•	Ask questions and get AI-generated answers from the document

⸻

API Endpoints

Upload PDF

POST /pdf/upload

Example response:
{
  "message": "PDF uploaded successfully",
  "sessionId": "123abc"
}

Ask Question

GET /chat

Example:
/chat?sessionId=123abc&question=What is the document about?

Architecture

PDF → Text Extraction → Chunking → Embeddings → Vector DB
→ Similarity Search → Gemini AI → Answer

⸻

Future Improvements
	•	Authentication for users
	•	UI for uploading and chatting
	•	Support multiple documents
	•	Deploy on cloud

⸻

Author

Manoj Thangaraj

Backend Developer | Java | Spring Boot | AI Integration
