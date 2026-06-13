<img width="1536" height="1024" alt="ChatGPT Image Jun 13, 2026, 11_04_13 PM" src="https://github.com/user-attachments/assets/65d6a15b-a42d-4e50-98ce-b688e92506ec" />
<img width="1905" height="946" alt="image" src="https://github.com/user-attachments/assets/ca30525e-109a-45e7-9823-bcd7c9b307c9" />
<img width="1905" height="941" alt="image" src="https://github.com/user-attachments/assets/00c1834a-6303-4f52-8582-c859e459714a" />
<img width="1906" height="946" alt="image" src="https://github.com/user-attachments/assets/5d00cd33-cd21-4976-91d1-c5bd09ad8d95" />
<img width="1909" height="939" alt="image" src="https://github.com/user-attachments/assets/125d8ce7-007f-4578-83ed-60a89b37e49b" />

<div align="center">

# 🧠 LUMIVRA AI

### Intelligent AI Coding Companion + Local AI Music Studio

AI Chat • Code Execution • AI Memory • Voice Cloning • Voice Swap • Music Processing

![Lumivra AI Banner](./assets/lumivra-showcase.png)

</div>

---

## 🚀 Overview

LUMIVRA AI is a full-stack AI platform that combines:

- GPT-style conversational AI
- In-browser code execution
- Persistent AI memory
- File analysis & vision
- Local AI music processing
- Voice cloning & voice swapping

Everything is integrated into a single modern interface built with Next.js, Supabase, Groq, FastAPI and PyTorch.

---

## ✨ Core Features

### 💬 AI Chat

- Real-time streaming responses
- Multiple AI models
- Message editing & regeneration
- Markdown support
- Syntax highlighting
- AI-generated chat titles

### 🧠 AI Memory

- Remembers user preferences
- Cross-chat persistence
- Smart memory extraction
- Memory management dashboard

### ⚡ Code Execution

Run code directly inside chat.

Supported:

- JavaScript
- Python (Pyodide)

Features:

- Interactive input
- Console output
- Error capture

### 📎 File Support

Upload:

- PDF
- DOCX
- TXT
- Images
- Code files
- CSV / JSON

### 👁️ Vision AI

Analyze images using Llama 4 Scout.

- Image understanding
- Screenshot analysis
- Visual reasoning

### 🎵 Music Studio

#### Vocal Separation

Split songs into:

- Vocals
- Instrumentals

Powered by Demucs.

#### Voice Training

Train AI using your own voice.

#### Voice Swap

Replace a singer's voice with your own.

#### Audio Controls

- Pitch shifting
- Similarity control
- Volume mixing
- Audio preview

### 🔒 Privacy First

Music processing runs locally.

- No audio uploads
- GPU accelerated
- Apple Silicon support
- NVIDIA CUDA support

---

## 🛠️ Tech Stack

### Frontend

- Next.js 16
- TypeScript
- Mantine UI
- Zustand

### Backend

- Supabase
- Groq Cloud
- FastAPI

### AI

- Llama 3.3 70B
- Llama 4 Scout
- Mixtral 8x7B
- Gemma 2 9B

### Audio AI

- Demucs
- HuBERT
- RVC v2
- FFmpeg
- PyTorch

---

## 🏗️ Architecture

```text
Frontend (Next.js)
        │
        ▼
   Groq Cloud
        │
        ▼
   Supabase DB
        │
        ▼
 FastAPI Music Server
        │
 ┌──────┼──────┐
 ▼      ▼      ▼
Demucs HuBERT RVC
```

---

## 📊 Project Highlights

| Metric | Value |
|----------|----------|
| Features | 20+ |
| AI Models | 5 |
| Supported File Types | 10+ |
| Lines of Code | 8000+ |
| Database Tables | 4 |
| Music Processing | 100% Local |

---

## 🎯 Built For

- Developers
- Students
- Researchers
- Content Creators
- Music Producers

---

## 🚀 Quick Start

```bash
git clone https://github.com/yourusername/lumivra-ai.git

cd lumivra-ai

pnpm install

pnpm dev
```

Run Music Server:

```bash
cd music-server

pip install -r requirements.txt

python server.py
```

---

## 🗺️ Roadmap

- [ ] Voice Input
- [ ] Chat Sharing
- [ ] PDF Export
- [ ] Keyboard Shortcuts
- [ ] Message Search
- [ ] Waveform Visualization
- [ ] Token Analytics

---

## 📸 Screenshots

Add screenshots here.

```md
![Chat](./screenshots/chat.png)

![Music Studio](./screenshots/music.png)

![AI Memory](./screenshots/memory.png)
```

---

## 👨‍💻 Author

**Gautham Jayesh**

GitHub: https://github.com/yourusername

---

## ⭐ Why This Project?

LUMIVRA AI combines the capabilities of:

- ChatGPT
- LALAL.AI
- ElevenLabs
- Kits.ai
- Musicfy

into a single integrated platform focused on privacy, local processing, and AI-powered productivity.


## 📁 Project Structure

```text
lumivra-ai
│
├── app/                     # Next.js App Router
│   ├── api/                 # Backend API routes
│   ├── chat/                # AI Chat UI
│   ├── music/               # Music Studio
│   ├── settings/            # User settings
│   └── (auth)/              # Login & signup
│
├── components/
│   ├── chat/                # Chat components
│   ├── music/               # Music Studio UI
│   └── sidebar/             # Navigation
│
├── lib/
│   ├── supabase/            # Database helpers
│   ├── hooks/               # Custom hooks
│   ├── contexts/            # React contexts
│   ├── codeRunner.ts        # JS/Python execution
│   ├── fileParser.ts        # File processing
│   └── musicApi.ts          # Music server client
│
├── store/
│   └── chatStore.ts         # Zustand state
│
├── types/
│   └── index.ts             # Shared types
│
├── music-server/            # Python AI Backend
│   ├── server.py            # FastAPI server
│   ├── separator.py         # Demucs processing
│   ├── trainer.py           # Voice training
│   ├── converter.py         # Voice conversion
│   ├── mixer.py             # Audio mixing
│   └── rvc_wrapper.py       # RVC integration
│
├── public/
│   ├── screenshots/
│   └── assets/
│
├── package.json
├── tsconfig.json
├── next.config.ts
├── middleware.ts
└── README.md
```

### Architecture Overview

```text
┌─────────────────────────────┐
│       Next.js Frontend      │
│   Chat • Memory • Music UI  │
└──────────────┬──────────────┘
               │
      ┌────────┴────────┐
      │                 │
      ▼                 ▼

┌───────────────┐  ┌─────────────────┐
│  Groq Cloud   │  │    Supabase     │
│   AI Models   │  │ Auth + Database │
└───────────────┘  └─────────────────┘

               │
               ▼

┌─────────────────────────────┐
│    FastAPI Music Server     │
└──────────────┬──────────────┘
               │
      ┌────────┼────────┐
      ▼        ▼        ▼

   Demucs    HuBERT    RVC
 Vocal Sep  Features  Voice AI
```

### Key Modules

| Module | Purpose |
|----------|----------|
| AI Chat | GPT-style conversation |
| AI Memory | Persistent user memory |
| Code Runner | Execute JS & Python |
| Vision AI | Analyze uploaded images |
| File Processing | PDF, DOCX, Code & Data |
| Music Studio | Vocal separation & voice swap |
| Authentication | Email + Google OAuth |
| Database Layer | Chats, memories & settings |

<div align="center">

### 🚀 DEVELOPED BY GAUTHAM JAYESH 🚀

**Next.js 16 • TypeScript • Supabase • Groq Cloud • Mantine UI • Pyodide**

## License

Copyright © 2026 Gautham Jayesh.

This repository is published for portfolio and demonstration purposes only.

Lumivra AI is a personal project published to showcase my software engineering, AI integration, and full-stack development skills. The source code is not open source and may not be copied, modified, redistributed, or used without permission.

</div>
