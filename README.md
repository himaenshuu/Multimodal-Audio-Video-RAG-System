# 🎯 Audio-Video RAG with Gemini & Qdrant

This project implements a **Retrieval-Augmented Generation (RAG)** system that accepts audio or video input, transcribes it, and performs question-answering using **Google Gemini** and **Qdrant**.

### 🚀 Features
- Transcribe audio using **Faster-Whisper**
- Extract and convert audio from videos via **FFmpeg**
- Semantic retrieval using **LangChain + Qdrant**
- Answer generation using **Google Gemini Pro**
- Supports `.mp3`, `.wav`, and `.mp4` files

### 🧰 Tech Stack Used

This project integrates audio/video data with a RAG pipeline using modern tools and frameworks:

| Technology | Logo | Purpose |
|------------|------|---------|
| [Python](https://www.python.org/) | ![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white) | Backend logic and orchestration |
| [LangChain](https://www.langchain.com/) | ![LangChain](https://img.shields.io/badge/LangChain-000000?style=for-the-badge&logo=langchain&logoColor=white) | RAG architecture and LLM interface |
| [Gemini (Google Generative AI)](https://ai.google.dev/) | ![Gemini](https://img.shields.io/badge/Gemini%20AI-4285F4?style=for-the-badge&logo=google&logoColor=white) | LLM and Embeddings |
| [Qdrant](https://qdrant.tech/) | ![Qdrant](https://img.shields.io/badge/Qdrant-3F3D56?style=for-the-badge&logo=qdrant&logoColor=white) | Vector database for semantic search |
| [Faster-Whisper](https://github.com/guillaumekln/faster-whisper) | ![Whisper](https://img.shields.io/badge/Faster--Whisper-0066CC?style=for-the-badge&logo=whisper&logoColor=white) | Fast local speech-to-text model |
| [FFmpeg](https://ffmpeg.org/) | ![FFmpeg](https://img.shields.io/badge/FFmpeg-007808?style=for-the-badge&logo=ffmpeg&logoColor=white) | Audio extraction from video files |
| [Jupyter Notebook](https://jupyter.org/) | ![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge&logo=jupyter&logoColor=white) | Interactive development environment |


### 🔧 Requirements
- Python = 3.10  
- FFmpeg (added to PATH)  
- Gemini API Key  
- Install dependencies:
- pip install -r requirements.txt



## Appendices

# 🎬 FFmpeg Installation Guide
---

## ✅ Windows Installation

1. **Download FFmpeg**:
   - Visit: [https://www.gyan.dev/ffmpeg/builds/](https://www.gyan.dev/ffmpeg/builds/)
   - Under “Release builds”, download **`ffmpeg-release-full.7z`** or **`ffmpeg-release-essentials.zip`**

2. **Extract the Archive**:
   - Use [7-Zip](https://www.7-zip.org/) or WinRAR to extract the file
   - Extract the contents to `C:\ffmpeg`

3. **Add to System PATH**:
   - Open:
     - `Control Panel` → `System` → `Advanced system settings` → `Environment Variables`
   - Under **System variables**, find `Path` → Click **Edit**
   - Click **New** and enter: `C:\ffmpeg\bin`
   - Click **OK** to save

4. **Verify Installation**:
   - Open Command Prompt and run:
     ```bash
     ffmpeg -version
     
