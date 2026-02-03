# Aureeq - AI Sales Restaurant Agent

Aureeq is an intelligent, voice-activated AI sales assistant designed for **IYI Restaurant**. It combines a 3D avatar frontend with a powerful local LLM backend to engage customers, answer menu queries, and upsell items using professional sales strategies.

## Project Structure

- **frontend/**: A modern web interface featuring a 3D VRM avatar (Three.js), speech recognition, and lip-sync capabilities. Built with Vite.
- **model_training/**: The Python backend (FastAPI) that powers the AI. It uses:
  - **Ollama (Llama 3)** for intelligence.
  - **ChromaDB** for RAG (Retrieval Augmented Generation) to access the menu and sales examples.
  - **Edge TTS** for voice synthesis.
- **data/**: Contains menu data, voice samples, and vector store artifacts.

## Quick Start

### 1. Backend (Python)
Navigate to `model_training/scripts` and run the server:
```bash
cd model_training/scripts
python server.py
```
*Server runs on http://localhost:8001*

### 2. Frontend (Node.js)
Navigate to `frontend` and start the dev server:
```bash
cd frontend
npm run dev
```
*App runs on http://localhost:5173*

## Features
- **Voice Interaction**: Talk to Aureeq naturally using the microphone.
- **3D Avatar**: Fully animated avatar with lip-sync.
- **RAG Sales Brain**: Trained on 400+ specific sales examples to "romance the food" and upsell effectively.
- **Menu Knowledge**: Full awareness of the IYI Restaurant menu, ingredients, and pricing.
