# 🎯 Audio-Video RAG with Gemini & Qdrant

This project implements a **Retrieval-Augmented Generation (RAG)** system that accepts audio or video input, transcribes it, and performs question-answering using **Google Gemini** and **Qdrant**.

### 🚀 Features
- Transcribe audio using **Faster-Whisper**
- Extract and convert audio from videos via **FFmpeg**
- Semantic retrieval using **LangChain + Qdrant**
- Answer generation using **Google Gemini Pro**
- Supports `.mp3`, `.wav`, and `.mp4` files

### 🔧 Requirements
- Python = 3.10  
- FFmpeg (added to PATH)  
- Gemini API Key  
- Install dependencies:
```bash
pip install -r requirements.txt
