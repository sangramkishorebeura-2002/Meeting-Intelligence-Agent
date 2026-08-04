# Meeting Intelligence Agent

An AI-powered Meeting Intelligence Platform that transforms meeting recordings, YouTube videos, and audio files into actionable business insights using Large Language Models (LLMs), Retrieval-Augmented Generation (RAG), and automated meeting analytics.

## Overview

Meeting Intelligence Agent automates the entire post-meeting workflow:

* Meeting transcription
* AI-generated summaries
* Action item extraction
* Key decision tracking
* Open question identification
* Conversational meeting search using RAG
* Interactive Streamlit dashboard

The system supports English, Hindi, and Hinglish meetings through local Whisper transcription and Sarvam AI speech-to-text translation.

---

## Features

### Meeting Transcription

* Upload audio or video recordings
* Process YouTube URLs
* English transcription using OpenAI Whisper
* Hindi/Hinglish transcription using Sarvam AI

### AI Meeting Summaries

Generate concise meeting summaries with:

* Key discussion points
* Important updates
* Meeting outcomes
* Executive-level overviews

### Action Item Extraction

Automatically identifies:

* Tasks
* Owners
* Deadlines
* Follow-up responsibilities

### Key Decision Tracking

Captures important business decisions discussed during meetings.

### Open Questions Detection

Identifies:

* Unresolved discussions
* Pending approvals
* Follow-up topics

### RAG-Based Meeting Chat

Ask questions such as:

* What decisions were made?
* What deadlines were discussed?
* What did the marketing team agree on?
* Who owns a specific task?

The assistant retrieves relevant meeting context using ChromaDB and semantic search.

---

## Architecture

Input Source
↓
Audio Processing
↓
Whisper / Sarvam AI
↓
Transcript Generation
↓
AI Summarization
↓
Action Item Extraction
↓
Decision Extraction
↓
Question Extraction
↓
Vector Database (ChromaDB)
↓
RAG Pipeline
↓
Meeting Intelligence Dashboard

---

## Tech Stack

### Artificial Intelligence

* Mistral AI
* OpenAI Whisper
* Sarvam AI

### LLM Framework

* LangChain LCEL

### Retrieval-Augmented Generation

* ChromaDB
* HuggingFace Embeddings
* Semantic Search

### Backend

* Python

### User Interface

* Streamlit

### NLP

* Text Summarization
* Information Extraction
* Retrieval-Augmented Generation

---

## Project Structure

```text
Meeting-Intelligence-Agent/
│
├── app.py
├── main.py
├── Requirements.txt
│
├── core/
│   ├── transcriber.py
│   ├── summarizer.py
│   ├── extractor.py
│   ├── rag_engine.py
│   └── vector_store.py
│
└── utils/
    └── audio_processor.py
```

---

## Installation

### Clone Repository

```bash
git clone https://github.com/mr-akash12/Meeting-Intelligence-Agent.git

cd Meeting-Intelligence-Agent
```

### Create Virtual Environment

```bash
python -m venv .venv
```

### Activate Environment

Windows

```bash
.venv\Scripts\activate
```

### Install Dependencies

```bash
pip install -r Requirements.txt
```

---

## Environment Variables

Create a `.env` file:

```env
MISTRAL_API_KEY=your_mistral_api_key
SARVAM_API_KEY=your_sarvam_api_key
```

---

## Run Application

```bash
streamlit run app.py
```

---

## Example Workflow

1. Upload meeting recording or provide YouTube URL.
2. Generate transcript.
3. Create AI summary.
4. Extract action items.
5. Extract key decisions.
6. Detect open questions.
7. Chat with the meeting using RAG.

---

## Business Use Cases

* Executive Meeting Analysis
* Project Status Reviews
* Client Discovery Calls
* Sales Meetings
* Product Planning Sessions
* Team Standups
* Recruitment Interviews

---

## Future Enhancements

* LangGraph Multi-Agent Architecture
* Speaker Diarization
* Follow-up Email Generation
* Meeting Sentiment Analysis
* Calendar Integration
* Slack Notifications
* Meeting Analytics Dashboard
* Team Productivity Metrics

---

## Author

Akash Kumar Nayak

Generative AI Engineer | Data Scientist | AI/ML Engineer

Focused on Generative AI, Agentic AI Systems, RAG Pipelines, NLP, and Enterprise Automation.
