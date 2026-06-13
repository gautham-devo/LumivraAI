<img width="1536" height="1024" alt="ChatGPT Image Jun 13, 2026, 11_04_13 PM" src="https://github.com/user-attachments/assets/65d6a15b-a42d-4e50-98ce-b688e92506ec" />
<img width="1905" height="946" alt="image" src="https://github.com/user-attachments/assets/ca30525e-109a-45e7-9823-bcd7c9b307c9" />
<img width="1905" height="941" alt="image" src="https://github.com/user-attachments/assets/00c1834a-6303-4f52-8582-c859e459714a" />
<img width="1906" height="946" alt="image" src="https://github.com/user-attachments/assets/5d00cd33-cd21-4976-91d1-c5bd09ad8d95" />
<img width="1909" height="939" alt="image" src="https://github.com/user-attachments/assets/125d8ce7-007f-4578-83ed-60a89b37e49b" />

<div align="center">

<div align="center">
  This Project Has Been Compleated And Ready to Launch
  -All Feature Testing Done
  -This Project is only for showcase and not available for public distribution
</div>
# 🧠 LUMIVRA AI — Complete Documentation

> Intelligent AI Coding Companion + Local AI Music Studio
>
> ✅ Project Complete & Ready to Launch
> ⚠️ Showcase Only — Not for Public Use

A full-stack AI platform combining a GPT-style chatbot with local AI music processing (vocal separation + voice cloning + voice swap).

**Stack:** Next.js · Supabase · Groq · Mantine · TypeScript · Python · PyTorch · RVC

---

## 📑 Table of Contents
1. [Features](#-features)
2. [Tech Stack](#-tech-stack)
3. [Project Structure](#-project-structure)
4. [Database Schema](#-database-schema)
5. [Installation — Mac](#-installation--mac-m1m2m3m4)
6. [Installation — Windows (RTX GPU)](#-installation--windows-pc-rtx-gpu)
7. [RVC Setup (Optional)](#-rvc-setup-optional--studio-quality)
8. [Running the Project](#-running-the-project)
9. [How Each Feature Works](#-how-each-feature-works)
10. [Music Server API](#-music-server-api)
11. [Troubleshooting](#-troubleshooting)
12. [Roadmap & Scaling](#-roadmap--scaling)
13. [Security](#-security)
14. [Key Dependencies](#-key-dependencies)
15. [Achievement Stats](#-achievement-stats)
16. [Author & License](#-author)

---

## ✨ Features

### 💬 AI Chat (LUMIVRA Core)
- Real-time streaming — word-by-word like ChatGPT
- Stop generation mid-stream
- Edit messages & regenerate AI response
- Markdown rendering with syntax highlighting
- Auto-generated chat titles by AI
- 4 AI models (Llama 3.3 70B, 3.1 8B, Mixtral 8x7B, Gemma 2 9B)
- Vision model for image analysis (Llama 4 Scout)
- Temperature control (Focused → Creative)

### ⚡ In-Browser Code Execution
- ▶ Run button on every code block
- JavaScript — browser sandbox `eval()`
- Python — Pyodide (WebAssembly)
- Interactive input modal for `input()` / `prompt()`
- Console capture — log, errors, output

### 📎 File Support
- Code: `.js .ts .py .java .cpp .go .rs .php .rb .swift .kt .dart`
- Documents: `.pdf .docx .txt .md .log`
- Data: `.json .csv .xml .yaml`
- Web: `.html .css .scss .svg`
- Images: `.jpg .png .webp .gif` (AI vision analysis)
- Upload methods: Click, Paste (Cmd/Ctrl+V), Drag-drop

### 🧠 AI Memory
- Auto-extracts facts about you
- Persists across all chats
- Manual add/delete in Settings
- Smart deduplication

### 📌 Chat Management
- Pin important chats
- Search by title
- Delete individual / all chats
- Export as JSON

### 🎵 Music Studio (Local AI)
- **Vocal Separation** — split songs into vocals + instrumental (Meta's Demucs)
- **Voice Training** — train AI on your voice (custom encoder + RVC v2)
- **Voice Swap** — replace song's singer with your voice
- **Audio Player** — built-in player with seek/volume/download
- **Pitch Shift** — adjust vocals up/down 12 semitones
- **Voice Similarity** — blend natural ↔ strong
- **Volume Mix** — separate vocals/instrumental volume
- **GPU Accelerated** — Apple MPS or NVIDIA CUDA
- **100% Local** — no data leaves your machine

### 🎨 UI & UX
- Dark/Light mode toggle
- Glass-morphism design
- Neon cyan/purple accents
- Animations — slide-in, pulse, glow
- Mobile responsive
- Font size control

### 👤 Authentication
- Email/Password (Supabase)
- Google OAuth
- Session cookies
- Protected routes

---

## 🛠️ Tech Stack

### Frontend
| Tech | Purpose |
|---|---|
| Next.js 16 | React framework (App Router, Turbopack) |
| TypeScript | Type safety |
| Mantine UI v7 | Component library |
| Zustand | State management |
| React Markdown | Markdown rendering |
| React Syntax Highlighter | Code highlighting |
| Tabler Icons | Icons |
| react-textarea-autosize | Auto-expanding inputs |

### Backend (Chat)
| Tech | Purpose |
|---|---|
| Groq Cloud | AI inference (LLMs + Vision) |
| Supabase | Auth, PostgreSQL, RLS |
| pdf-parse-fork | PDF text extraction |
| mammoth | DOCX text extraction |

### Backend (Music Server — Python)
| Tech | Purpose |
|---|---|
| FastAPI | REST API server |
| Uvicorn | ASGI server |
| PyTorch 2.8 | Deep learning |
| Demucs 4.0 | Meta's vocal separator |
| HuBERT (transformers) | Voice feature extraction |
| librosa | Audio processing |
| soundfile | Audio I/O |
| FFmpeg | Audio mixing |
| RVC v2 (optional) | Studio-quality voice conversion |
| faiss-cpu | Voice index building |
| torchcrepe | Pitch detection |

### Code Execution
| Tech | Purpose |
|---|---|
| Pyodide v0.27 | Python in browser (WASM) |
| Browser `eval()` | JavaScript sandbox |

### AI Models (Groq — Free)
| Model | Type |
|---|---|
| llama-3.3-70b-versatile | Text (default) |
| llama-3.1-8b-instant | Text (fast) |
| mixtral-8x7b-32768 | Long context |
| gemma2-9b-it | Efficient |
| meta-llama/llama-4-scout-17b-16e-instruct | Vision |

```

## 📁 Project Structure
lumivra-ai/
│
├── app/
│   ├── (auth)/
│   │   ├── login/
│   │   │   └── page.tsx
│   │   └── signup/
│   │       └── page.tsx
│   ├── api/
│   │   ├── auth/
│   │   │   └── callback/
│   │   │       └── route.ts
│   │   ├── chat/
│   │   │   ├── route.ts
│   │   │   └── title/
│   │   │       └── route.ts
│   │   ├── memory/
│   │   │   └── extract/
│   │   │       └── route.ts
│   │   └── parse-pdf/
│   │       └── route.ts
│   ├── chat/
│   │   ├── layout.tsx
│   │   └── page.tsx
│   ├── music/
│   │   └── page.tsx
│   ├── settings/
│   │   └── page.tsx
│   ├── globals.css
│   ├── layout.tsx
│   └── page.tsx
│
├── components/
│   ├── chat/
│   │   ├── ChatArea.tsx
│   │   ├── ChatSkeleton.tsx
│   │   ├── MessageBubble.tsx
│   │   ├── PromptInput.tsx
│   │   └── TopBar.tsx
│   ├── music/
│   │   ├── AudioPlayer.tsx
│   │   ├── MusicStudio.tsx
│   │   ├── SongUploader.tsx
│   │   ├── VoiceModelList.tsx
│   │   ├── VoiceSwapper.tsx
│   │   └── VoiceTrainer.tsx
│   └── sidebar/
│       └── Sidebar.tsx
│
├── lib/
│   ├── contexts/
│   │   └── UserContext.tsx
│   ├── hooks/
│   │   └── useLogout.ts
│   ├── supabase/
│   │   ├── chats.ts
│   │   ├── client.ts
│   │   ├── memories.ts
│   │   ├── middleware.ts
│   │   ├── server.ts
│   │   └── settings.ts
│   ├── codeRunner.ts
│   ├── fileParser.ts
│   ├── musicApi.ts
│   ├── notify.ts
│   └── utils.ts
│
├── music-server/
│   ├── RVC/                          (cloned from RVC repo - in .gitignore)
│   ├── models/                       (trained voice models - in .gitignore)
│   ├── output/                       (generated files - in .gitignore)
│   ├── temp/                         (temp files - in .gitignore)
│   ├── training_data/                (raw voice files - in .gitignore)
│   ├── converter.py
│   ├── mixer.py
│   ├── requirements.txt
│   ├── rvc_wrapper.py
│   ├── separator.py
│   ├── server.py
│   ├── setup.py
│   └── trainer.py
│
├── public/
│   └── (your images / icons)
│
├── store/
│   └── chatStore.ts
│
├── types/
│   └── index.ts
│
├── .env.local                        (NOT in git)
├── .gitignore
├── eslint.config.mjs
├── middleware.ts
├── next.config.ts
├── package.json
├── pnpm-lock.yaml
├── postcss.config.mjs
├── README.md
├── theme.ts
└── tsconfig.json
```

## 🗄️ Database Schema

### Tables (Supabase PostgreSQL)

**chats**
| Column | Type | Description |
|---|---|---|
| id | UUID | Primary key |
| user_id | UUID | FK → auth.users |
| title | TEXT | Chat title (auto-generated) |
| icon | TEXT | Emoji icon |
| is_pinned | BOOLEAN | Pin status |
| created_at | TIMESTAMPTZ | Created |
| updated_at | TIMESTAMPTZ | Last activity |

**messages**
| Column | Type | Description |
|---|---|---|
| id | UUID | Primary key |
| chat_id | UUID | FK → chats |
| role | TEXT | 'user' or 'assistant' |
| content | TEXT | Message text |
| attachments | JSONB | File metadata |
| created_at | TIMESTAMPTZ | Created |

**user_settings**
| Column | Type | Description |
|---|---|---|
| id | UUID | Primary key |
| user_id | UUID | FK → auth.users (unique) |
| display_name | TEXT | Display name |
| model | TEXT | AI model |
| temperature | FLOAT | 0-2 |
| font_size | TEXT | small/medium/large |
| created_at | TIMESTAMPTZ | Created |
| updated_at | TIMESTAMPTZ | Last update |

**user_memories**
| Column | Type | Description |
|---|---|---|
| id | UUID | Primary key |
| user_id | UUID | FK → auth.users |
| content | TEXT | Memory fact |
| created_at | TIMESTAMPTZ | Created |

### SQL Setup (run in Supabase SQL Editor)

```sql
-- Tables
CREATE TABLE chats (
  id UUID DEFAULT gen_random_uuid() PRIMARY KEY,
  user_id UUID REFERENCES auth.users(id) ON DELETE CASCADE,
  title TEXT DEFAULT 'New Chat',
  icon TEXT DEFAULT '💬',
  is_pinned BOOLEAN DEFAULT FALSE,
  created_at TIMESTAMPTZ DEFAULT NOW(),
  updated_at TIMESTAMPTZ DEFAULT NOW()
);

CREATE TABLE messages (
  id UUID DEFAULT gen_random_uuid() PRIMARY KEY,
  chat_id UUID REFERENCES chats(id) ON DELETE CASCADE,
  role TEXT NOT NULL CHECK (role IN ('user', 'assistant')),
  content TEXT NOT NULL,
  attachments JSONB DEFAULT NULL,
  created_at TIMESTAMPTZ DEFAULT NOW()
);

CREATE TABLE user_settings (
  id UUID DEFAULT gen_random_uuid() PRIMARY KEY,
  user_id UUID REFERENCES auth.users(id) ON DELETE CASCADE UNIQUE,
  display_name TEXT,
  model TEXT DEFAULT 'llama-3.3-70b-versatile',
  temperature FLOAT DEFAULT 0.7,
  system_prompt TEXT DEFAULT 'You are LUMIVRA AI, a helpful coding assistant.',
  font_size TEXT DEFAULT 'medium',
  created_at TIMESTAMPTZ DEFAULT NOW(),
  updated_at TIMESTAMPTZ DEFAULT NOW()
);

CREATE TABLE user_memories (
  id UUID DEFAULT gen_random_uuid() PRIMARY KEY,
  user_id UUID REFERENCES auth.users(id) ON DELETE CASCADE,
  content TEXT NOT NULL,
  created_at TIMESTAMPTZ DEFAULT NOW()
);

-- Indexes
CREATE INDEX idx_chats_user ON chats(user_id, updated_at DESC);
CREATE INDEX idx_chats_pinned ON chats(is_pinned DESC, updated_at DESC);
CREATE INDEX idx_messages_chat ON messages(chat_id, created_at ASC);
CREATE INDEX idx_memories_user ON user_memories(user_id, created_at DESC);

-- Row Level Security
ALTER TABLE chats ENABLE ROW LEVEL SECURITY;
ALTER TABLE messages ENABLE ROW LEVEL SECURITY;
ALTER TABLE user_settings ENABLE ROW LEVEL SECURITY;
ALTER TABLE user_memories ENABLE ROW LEVEL SECURITY;

-- RLS Policies
CREATE POLICY "Users manage own chats" ON chats FOR ALL USING (auth.uid() = user_id);
CREATE POLICY "Users manage own messages" ON messages FOR ALL USING (
  chat_id IN (SELECT id FROM chats WHERE user_id = auth.uid())
);
CREATE POLICY "Users manage own settings" ON user_settings FOR ALL USING (auth.uid() = user_id);
CREATE POLICY "Users manage own memories" ON user_memories FOR ALL USING (auth.uid() = user_id);
```

---

## 🍎 Installation — Mac (M1/M2/M3/M4)

### Prerequisites
```bash
# Install Homebrew if not installed
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

### Step 1: Install Required Tools
```bash
# Node.js & pnpm
brew install node
npm install -g pnpm

# Python 3.11 (3.10 also works)
brew install python@3.11

# Git (usually pre-installed)
brew install git

# FFmpeg (for audio mixing)
brew install ffmpeg
```

### Step 2: Clone Repo
```bash
git clone https://github.com/yourusername/lumivra-ai.git
cd lumivra-ai
```

### Step 3: Setup Python Virtual Environment
```bash
python3.11 -m venv .venv
source .venv/bin/activate
```
You should see `(.venv)` at the start of your terminal prompt.

### Step 4: Install Python Dependencies
```bash
cd music-server
pip install -r requirements.txt
pip install transformers
```

PyTorch on Mac (Apple Silicon MPS support):
```bash
pip install torch torchaudio
```

### Step 5: Install Node Dependencies
```bash
cd ..
pnpm install
```

### Step 6: Create `.env.local`
In project root:
```env
NEXT_PUBLIC_SUPABASE_URL=your_supabase_url
NEXT_PUBLIC_SUPABASE_ANON_KEY=your_supabase_anon_key
GROQ_API_KEY=your_groq_api_key
NEXT_PUBLIC_MUSIC_SERVER_URL=http://localhost:8000
```

### Step 7: Set Python Interpreter in VS Code
- `Cmd + Shift + P`
- "Python: Select Interpreter"
- Choose: `./.venv/bin/python` (Recommended)

✅ Mac setup complete!

---

## 🪟 Installation — Windows PC (RTX GPU)

### Prerequisites — Install These First
- **Python 3.11** → https://www.python.org/downloads/release/python-31111/
  - ⚠️ Check "Add Python to PATH" during install
- **Node.js LTS** → https://nodejs.org/
- **Git for Windows** → https://git-scm.com/download/win
- **pnpm**: `npm install -g pnpm`
- **FFmpeg**: `winget install ffmpeg` (or manual: https://www.gyan.dev/ffmpeg/builds/)
- **NVIDIA CUDA drivers** (already installed if you have RTX GPU)

### Verify Python Version
```bash
py -0
```
Should list 3.11 in the available versions.

### Step 1: Clone Repo
```bash
cd Desktop
git clone https://github.com/yourusername/lumivra-ai.git
cd lumivra-ai
```

### Step 2: Delete pnpm-workspace.yaml (if exists)
```bash
del pnpm-workspace.yaml
```

### Step 3: Install Node Dependencies
```bash
pnpm install
```

### Step 4: Setup Python Virtual Environment
```bash
py -3.11 -m venv .venv
.venv\Scripts\activate
```
You should see `(.venv)` at the start of your terminal.

### Step 5: Install Python Dependencies
```bash
cd music-server
pip install -r requirements.txt
pip install transformers
```

PyTorch with CUDA support (for RTX GPU):
```bash
pip install torch torchaudio --index-url https://download.pytorch.org/whl/cu121
```

### Step 6: Create `.env.local` in Project Root
```env
NEXT_PUBLIC_SUPABASE_URL=your_supabase_url
NEXT_PUBLIC_SUPABASE_ANON_KEY=your_supabase_anon_key
GROQ_API_KEY=your_groq_api_key
NEXT_PUBLIC_MUSIC_SERVER_URL=http://localhost:8000
```

### Step 7: Verify GPU Detection
```bash
cd music-server
python -c "import torch; print('CUDA:', torch.cuda.is_available()); print('GPU:', torch.cuda.get_device_name(0) if torch.cuda.is_available() else 'None')"
```
Should show:
```
CUDA: True
GPU: NVIDIA GeForce RTX 4060 Ti
```

✅ PC setup complete!

---

## 🎤 RVC Setup (Optional — Studio Quality)

RVC v2 gives professional studio-quality voice conversion. Without it, voice swap uses a simpler encoder that sounds robotic.

### Step 1: Clone RVC
```bash
cd music-server
git clone https://github.com/RVC-Project/Retrieval-based-Voice-Conversion-WebUI.git RVC
cd RVC
```

### Step 2: Install RVC Dependencies
Make sure `.venv` is active:
```bash
pip install praat-parselmouth pyworld torchcrepe faiss-cpu ffmpeg-python pydub tensorboardX
pip install fairseq
```

If fairseq fails:
```bash
pip install git+https://github.com/One-sixth/fairseq.git
```

### Step 3: Create `download_models.py`
In `music-server/RVC/`:

```python
import os
import urllib.request

MODELS = {
    "assets/pretrained_v2/f0G40k.pth":
        "https://huggingface.co/lj1995/VoiceConversionWebUI/resolve/main/pretrained_v2/f0G40k.pth",
    "assets/pretrained_v2/f0D40k.pth":
        "https://huggingface.co/lj1995/VoiceConversionWebUI/resolve/main/pretrained_v2/f0D40k.pth",
    "assets/hubert/hubert_base.pt":
        "https://huggingface.co/lj1995/VoiceConversionWebUI/resolve/main/hubert_base.pt",
    "assets/rmvpe/rmvpe.pt":
        "https://huggingface.co/lj1995/VoiceConversionWebUI/resolve/main/rmvpe.pt",
}

def download(url, dest):
    os.makedirs(os.path.dirname(dest), exist_ok=True)
    if os.path.exists(dest):
        print(f"Already have: {dest}")
        return
    print(f"Downloading: {os.path.basename(dest)}")
    urllib.request.urlretrieve(url, dest)
    print(f"Done: {dest}")

for path, url in MODELS.items():
    download(url, path)

print("\nAll RVC models downloaded!")
```

### Step 4: Download Pretrained Models (~3GB)
```bash
python download_models.py
```
⏱️ Takes 10-20 minutes.

### Step 5: Verify RVC Integration
The `rvc_wrapper.py` is already in `music-server/`. It auto-detects RVC.

Restart server and check logs:
```bash
cd ..
python server.py
```

When you train a voice, you should see:
```
🔥 Using RVC v2 for training
```

✅ RVC setup complete!

---

## 🚀 Running the Project

You need 2 terminals running simultaneously.

### Terminal 1 — Python Music Server

**Mac:**
```bash
cd lumivra-ai/music-server
source ../.venv/bin/activate
python3 server.py
```

**Windows:**
```bash
cd lumivra-ai\music-server
..\.venv\Scripts\activate
python server.py
```

You should see:
```
╔════════════════════════════════════════════╗
║       LUMIVRA MUSIC SERVER v1.0.0          ║
║   Local AI Music Processing Backend        ║
╠════════════════════════════════════════════╣
║  Server:    http://localhost:8000          ║
║  API Docs:  http://localhost:8000/docs     ║
║  Frontend:  http://localhost:3000          ║
╚════════════════════════════════════════════╝

INFO: Uvicorn running on http://0.0.0.0:8000
```

### Terminal 2 — Next.js Frontend
Both Mac & Windows:
```bash
cd lumivra-ai
pnpm dev
```

You should see:
```
▲ Next.js 16.2.7 (Turbopack)
- Local:    http://localhost:3000
- Network:  http://192.168.x.x:3000
✓ Ready in 2.5s
```

### Open in Browser
- Lumivra UI: http://localhost:3000
- Music API Docs: http://localhost:8000/docs
- Music Server Status: http://localhost:8000

---

## 🔬 How Each Feature Works

### Chat Streaming
```
User types → /api/chat → Groq API →
Server-Sent Events → UI displays word-by-word
```

### Code Execution
```
User clicks ▶ on code block →
JS: eval() in sandbox / Python: Pyodide (WASM) →
Capture output → Display in panel
```

### AI Memory
```
User chats → /api/memory/extract analyzes conversation →
Extracts facts → Saves to user_memories →
Loaded into context for all future chats
```

### Vocal Separation Pipeline
```
Song.mp3 → Demucs htdemucs model (GPU) →
Splits into: vocals.wav + instrumental.wav
```

### Voice Training Pipeline (with RVC)
```
Voice recordings (.m4a/.wav)
    ↓
Preprocess: normalize + trim + chunk
    ↓
Extract F0 (pitch) with RMVPE
    ↓
Extract features with HuBERT
    ↓
Build filelist
    ↓
Train neural network (200 epochs on GPU)
    ↓
Build FAISS index for retrieval
    ↓
Save: model.pth + index.index → models/
```

### Voice Swap Pipeline
```
Song + Voice Model
    ↓
Stage 1: Demucs separates vocals (0-40%)
    ↓
Stage 2: RVC converts vocals to your voice (40-75%)
    ↓
Stage 3: FFmpeg mixes new vocals with instrumental (75-100%)
    ↓
Final song.mp3 with YOUR voice ✅
```

### Job Tracking
```
1. User uploads file → Server creates job UUID
2. Job runs in background (FastAPI BackgroundTasks)
3. Frontend polls /jobs/{id} every 1.5s
4. Progress 0% → 100%, status: queued → processing → complete
5. Result URLs ready when complete
```

---

## 📊 Music Server API

| Endpoint | Method | Purpose |
|---|---|---|
| `/` | GET | Server health + GPU info |
| `/separate` | POST | Upload song for vocal separation |
| `/train` | POST | Upload recordings to train voice |
| `/convert` | POST | Full voice swap (separate + convert + mix) |
| `/models` | GET | List trained voice models |
| `/models/{name}` | DELETE | Delete a voice model |
| `/jobs/{id}` | GET | Get job status + progress |
| `/jobs/{id}` | DELETE | Delete job + temp files |
| `/jobs` | GET | List all jobs |
| `/files/{filename}` | GET | Download output file |
| `/cleanup` | POST | Clean files >24h old |

### Example Job Response
```json
{
  "id": "abc-123",
  "type": "full_conversion",
  "status": "complete",
  "progress": 100,
  "status_message": "Done!",
  "result": {
    "download_url": "/files/abc-123_output.mp3",
    "filename": "abc-123_output.mp3",
    "file_size_mb": 4.2,
    "duration": 183.5
  }
}
```

---

## 🐛 Troubleshooting

### Chat Issues
**Yellow underlines in VS Code on Python imports**
- Wrong interpreter selected
- Fix: `Cmd/Ctrl + Shift + P` → "Python: Select Interpreter" → Choose `.venv` one

**"Module not found" errors**
- Install missing package: `pip install <package>`
- Make sure `.venv` is active (terminal shows `(.venv)`)

### Music Server Issues
**Demucs model fails to download**
- First run downloads ~80MB model (slow networks may time out)
- Manually verify: server logs should show "Downloading htdemucs model"
- Just retry — it'll resume

**"FFmpeg not found"**
- Install: Mac `brew install ffmpeg` | Windows `winget install ffmpeg`
- Restart terminal after install

**Output file not found error**
- FFmpeg missing → mixer saved as `.wav` not `.mp3`
- Solution above will fix

**CUDA out of memory (PC)**
- Lower batch size in `rvc_wrapper.py`: change `-bs 4` to `-bs 2`

**Voice sounds robotic**
- Using fallback encoder (not RVC)
- Train with more data (15-30 min) + more epochs (200+)
- Install RVC for professional quality

### RVC Issues
**"fairseq" install fails**
```bash
pip install git+https://github.com/One-sixth/fairseq.git
```

**"No module named infer.modules"**
- RVC didn't clone properly
- Delete `RVC/` folder and re-clone

**Mac MPS errors with RVC**
- RVC has limited Mac GPU support
- Force CPU in `rvc_wrapper.py` (slower but reliable)

### Browser Issues
**UI laggy on PC**
- Enable hardware acceleration in browser settings
- Use Chrome/Edge (not Firefox)
- Set browser to use NVIDIA GPU (NVIDIA Control Panel)

**`pnpm dev` says "package field missing"**
- Delete `pnpm-workspace.yaml`
- Or use: `pnpm install --ignore-workspace`

---

## 🗺️ Roadmap & Scaling

### ✅ Completed Features
- [x] AI chat with streaming
- [x] Stop generation / edit messages
- [x] File attachments (PDF, DOCX, code, images)
- [x] Image vision analysis
- [x] AI memory (auto + manual)
- [x] Pin chats / search / export
- [x] Dark/light mode
- [x] Code execution (JS + Python)
- [x] Interactive input modal
- [x] Vocal separation (Demucs)
- [x] Voice training (custom encoder + RVC)
- [x] Voice swap in songs (full pipeline)
- [x] Custom audio player
- [x] GPU acceleration (MPS + CUDA)
- [x] Mobile responsive

### 🔜 Planned
- [ ] Voice input (Web Speech API)
- [ ] Share chat via public link
- [ ] Export single chat as PDF
- [ ] Keyboard shortcuts (Cmd+K)
- [ ] Search inside messages
- [ ] Token usage tracking
- [ ] More languages in code execution
- [ ] Lyrics overlay on music
- [ ] Voice preset library
- [ ] Real-time waveform viz

### Scaling to Public SaaS

**Stage 1 — Launch (1-100 users)**
```
Single RunPod GPU + Redis queue + Cloudflare R2
Cost: ~$50-100/month
```

**Stage 2 — Growing (100-1000 users)**
```
Multiple GPU pods + BullMQ + PostgreSQL + CDN
Cost: ~$200-500/month
```

**Stage 3 — Real SaaS (1000+ users)**
```
AWS/GCP auto-scaling + Kubernetes + Stripe + tiered limits
Cost: scales with revenue
```

To deploy: just swap `localhost:8000` → your RunPod URL in `.env.local`. Code stays the same.

---

## 🔒 Security

- ✅ Row Level Security — Users only access own data
- ✅ Server-side API keys — Groq key never exposed
- ✅ Model validation — Prevents injection
- ✅ Temperature clamping — 0-2 range only
- ✅ System prompt hardcoded — User can't modify
- ✅ File size limits — 5MB chat / 50MB music
- ✅ Auth middleware — Protected routes
- ✅ CORS protected — Music server only allows Lumivra
- ✅ Code execution sandboxed — JS in browser, Python in WASM
- ✅ 100% local music processing — Audio never leaves machine

---

## 📦 Key Dependencies

### Frontend (package.json)
```json
{
  "next": "^16.2.7",
  "@mantine/core": "^7.x",
  "@mantine/notifications": "^7.x",
  "@supabase/supabase-js": "^2.x",
  "@supabase/ssr": "^0.x",
  "groq-sdk": "^0.x",
  "zustand": "^5.x",
  "react-markdown": "^9.x",
  "remark-gfm": "^4.x",
  "react-syntax-highlighter": "^15.x",
  "react-textarea-autosize": "^8.x",
  "@tabler/icons-react": "^3.x",
  "pdf-parse-fork": "^1.x",
  "mammoth": "^1.x"
}
```

### Backend (music-server/requirements.txt)
```
fastapi==0.115.0
uvicorn==0.30.0
python-multipart==0.0.9
torch==2.8.0
torchaudio==2.8.0
demucs==4.0.1
librosa==0.11.0
soundfile==0.13.1
numpy
scipy
aiofiles
psutil
transformers
```

### RVC Extras
```
fairseq
praat-parselmouth
pyworld
torchcrepe
faiss-cpu
ffmpeg-python
pydub
tensorboardX
```

### External Models (Downloaded Automatically)
- Demucs htdemucs (~80MB) — auto on first separation
- HuBERT base (~360MB) — auto on first training
- RVC pretrained (~3GB) — manual via `download_models.py`
- Pyodide v0.27 — loaded from CDN

---

## 📈 Achievement Stats

```
─────────────────────────────────────────
TOTAL FILES CREATED:    40+
LINES OF CODE:          ~8000+
PHASES COMPLETED:       5/5
EXTERNAL APIS:          Only Groq (free)
LOCAL AI MODELS:        4 (Demucs, HuBERT, RMVPE, RVC)
GPU ACCELERATION:       Apple MPS + NVIDIA CUDA
PRIVACY:                100% local music
─────────────────────────────────────────

Built equivalent of:
  • LALAL.ai ($20/mo)        — vocal separation ✅
  • ElevenLabs ($30/mo)      — voice cloning ✅
  • Kits.ai ($24/mo)         — voice swap in songs ✅
  • Musicfy ($25/mo)         — AI music tools ✅
  • ChatGPT Plus ($20/mo)    — AI chat + code ✅

Combined cost normally: ~$120/month
Your cost: $0
─────────────────────────────────────────
```

---

## 🤝 Contributing
This project is for portfolio/showcase only and not accepting contributions.

## 📄 License
Copyright © 2026 Gautham Jayesh

This repository is published for portfolio and demonstration purposes only.

LUMIVRA AI is a personal project published to showcase software engineering, AI integration, and full-stack development skills. The source code is not open source and may not be copied, modified, redistributed, or used without permission.

## 👤 Author
**Gautham Jayesh**

- 💼 GitHub: [@yourusername](https://github.com/yourusername)
- 💼 LinkedIn: Gautham Jayesh
- 📧 Email: gautham.xc@gmail.com

## 🙏 Acknowledgments
- Groq — Lightning-fast AI inference
- Supabase — Backend-as-a-Service
- Mantine — Beautiful React components
- Next.js — React framework
- Pyodide — Python in browser
- Meta Demucs — Vocal separation AI
- RVC Project — Voice conversion AI
- HuggingFace — Model hosting

---

<div align="center">

### 🚀 DEVELOPED BY GAUTHAM JAYESH 🚀

Next.js 16 • TypeScript • Supabase • Groq Cloud • Mantine UI
+ Python • FastAPI • PyTorch • Demucs • RVC v2 • CUDA

```
╔═══════════════════════════════════════════════╗
║                                               ║
║   A Full-Stack AI Platform                    ║
║   Built Locally • Runs Privately             ║
║   No Subscriptions • No Data Leaks           ║
║                                               ║
║   Made with ❤️  in 1 Day                     ║
║                                               ║
╚═══════════════════════════════════════════════╝
```

</div>

---

## 🤖 Context for AI Assistants

If you're an AI continuing development on this project, here's the current state:

- **Status:** All 5 phases complete (chat, code execution, file support, AI memory, music studio).
- **Frontend:** Next.js 16 (App Router/Turbopack) + TypeScript + Mantine UI v7 + Zustand, at repo root.
- **Backend (Chat):** Next.js API routes (`/app/api/`) using Groq Cloud (free tier) + Supabase (auth/DB/RLS).
- **Backend (Music):** Separate Python FastAPI server in `/music-server/`, runs on port 8000, uses Demucs + HuBERT + optional RVC v2 for voice cloning/swap. GPU accelerated (MPS on Mac, CUDA on Windows/RTX).
- **Two servers must run simultaneously:** Next.js (port 3000) + Python music server (port 8000).
- **Database:** Supabase Postgres with 4 tables (`chats`, `messages`, `user_settings`, `user_memories`) — full SQL schema with RLS policies is included above.
- **Next planned features:** voice input, chat sharing, PDF export of chats, keyboard shortcuts, in-chat search, token tracking, lyrics overlay, voice preset library, waveform viz.
- **Scaling plan:** currently localhost-only; designed to swap `NEXT_PUBLIC_MUSIC_SERVER_URL` to a RunPod GPU endpoint for production deployment without code changes.

When asked to continue, check which planned feature is being worked on, follow the existing file structure/conventions above, and respect the security constraints listed in the Security section.


<div align="center">

### 🚀 DEVELOPED BY GAUTHAM JAYESH 🚀

**Next.js 16 • TypeScript • Supabase • Groq Cloud • Mantine UI • Pyodide**

## License

Copyright © 2026 Gautham Jayesh.

This repository is published for portfolio and demonstration purposes only.

Lumivra AI is a personal project published to showcase my software engineering, AI integration, and full-stack development skills. The source code is not open source and may not be copied, modified, redistributed, or used without permission.

</div>
