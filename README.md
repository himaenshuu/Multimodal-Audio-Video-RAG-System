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



## appendices

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
     ```
