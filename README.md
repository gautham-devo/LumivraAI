<img width="1536" height="1024" alt="ChatGPT Image Jun 10, 2026, 12_21_10 PM" src="https://github.com/user-attachments/assets/19a878ef-c4d6-4053-90a6-61d4df201911" />
<img width="1536" height="1024" alt="ChatGPT Image Jun 10, 2026, 12_40_41 PM" src="https://github.com/user-attachments/assets/807c460c-f1e0-4716-accb-65ba11caaaa5" />
<img width="2940" height="1912" alt="5CAEED17-824F-4151-9DB3-7BA9C1905292" src="https://github.com/user-attachments/assets/058c203f-7959-4786-add0-d6a50722e144" />
<img width="2940" height="1912" alt="DA34F663-6BBF-4E25-84C7-C6367DA5568C" src="https://github.com/user-attachments/assets/a0d56669-e77f-4a6a-8582-aadb2082de40" />


<div align="center">

<div align="center">
  This Project Has Been Compleated And Ready to Launch
  -All Feature Testing Done
  -This Project is only for showcase and not available for public distribution
</div>
# 🧠 LUMIVRA AI

### Your Intelligent AI Coding Companion

[![Next.js](https://img.shields.io/badge/Next.js-16-black?logo=next.js)](https://nextjs.org)
[![Supabase](https://img.shields.io/badge/Supabase-Database-3FCF8E?logo=supabase)](https://supabase.com)
[![Groq](https://img.shields.io/badge/Groq-AI%20Engine-orange)](https://groq.com)
[![Mantine](https://img.shields.io/badge/Mantine-UI-339AF0?logo=mantine)](https://mantine.dev)
[![TypeScript](https://img.shields.io/badge/TypeScript-Strict-3178C6?logo=typescript)](https://typescriptlang.org)

**A full-featured AI chatbot built with Next.js, Supabase, Groq Cloud, and Mantine UI.**  
**Supports streaming, file uploads, image analysis, AI memory, and in-browser code execution.**

[Live Demo](#) · [Report Bug](https://github.com/yourusername/lumivra-ai/issues) · [Request Feature](https://github.com/yourusername/lumivra-ai/issues)

</div>

## ✨ Features

### 💬 Chat & Messaging
- **Real-time streaming responses** — AI responses appear word-by-word like ChatGPT
- **Stop generation** — Cancel AI response mid-stream
- **Edit messages** — Modify sent messages and regenerate AI response
- **Markdown rendering** — Full markdown support with syntax highlighting
- **Code blocks** — Language-specific syntax highlighting with one-click copy
- **Auto-generated titles** — AI creates smart titles for each conversation

### ⚡ In-Browser Code Execution
- **▶ Run button** on every code block (JavaScript & Python)
- **Live output panel** — Shows results instantly below code
- **Input modal** — Interactive popup when code uses `input()` or `prompt()`
- **Auto input detection** — Extracts prompt text from code as labels
- **Multiple inputs supported** — Handle complex programs needing several inputs
- **Languages supported:**
  - 🟨 **JavaScript** — Runs instantly using browser eval (safe sandbox)
  - 🐍 **Python** — Powered by **Pyodide** (Python compiled to WebAssembly)
- **Console capture** — `console.log()`, `print()`, errors all shown in output
- **Cancel option** — Stop input modal anytime

### 📎 File Attachments
- **Click to attach** — File picker for all supported formats
- **Paste to attach** — Ctrl/Cmd+V to paste screenshots or files
- **Drag and drop** — Drag files directly onto the input area
- **Clean file chips** — Files show as compact chips (like ChatGPT), not raw content dumps
- **Supported formats:**
  - 💻 Code: `.js`, `.ts`, `.py`, `.java`, `.cpp`, `.go`, `.rs`, `.php`, `.rb`, `.swift`, `.kt`, `.dart` + more
  - 📝 Text: `.txt`, `.md`, `.log`
  - 📊 Data: `.json`, `.csv`, `.xml`, `.yaml`
  - 📕 PDF: Full text extraction (server-side parsing)
  - 📘 DOCX: Word document text extraction
  - 🌐 Web: `.html`, `.css`, `.scss`, `.svg`
  - 🖼️ Images: `.jpg`, `.png`, `.webp`, `.gif` (with AI vision analysis)

### 🖼️ Image Understanding
- **Upload screenshots** — AI analyzes images using Groq Vision model
- **Error analysis** — Upload screenshot of code errors → AI explains & fixes
- **UI analysis** — Upload UI mockups → AI describes and suggests improvements
- **Auto model switching** — Automatically uses vision model when images are detected
- **Vision model:** `meta-llama/llama-4-scout-17b-16e-instruct`

### 🧠 AI Memory
- **Automatic extraction** — AI picks up facts about you from conversations
- **Cross-chat memory** — Remembers your preferences across ALL chats
- **Manual control** — Add, view, and delete memories in Settings
- **Smart deduplication** — Won't store duplicate memories
- **Privacy first** — You see everything stored, delete anytime
- **Examples:** "User's name is Gautham", "Prefers TypeScript", "Building a startup"

### 📌 Chat Management
- **Pin important chats** — Pinned chats stay at the top of sidebar
- **Pinned/Recent sections** — Visual separation in sidebar
- **Delete individual chats** — Hover to see delete button
- **Delete all chats** — Nuclear option with confirmation modal
- **Search chats** — Filter chats by title
- **Export all chats** — Download as JSON file

### 🤖 AI Model Switching
- **4 Groq models available:**

  | Model | Best For |
  |---|---|
  | Llama 3.3 70B | Most powerful, balanced |
  | Llama 3.1 8B | Lightning fast responses |
  | Mixtral 8x7B | Long context window |
  | Gemma 2 9B | Google's efficient model |

- **Temperature control** — Slider from Focused (0) to Creative (2)
- **Persistent settings** — Saved to database per user

### 🎨 Appearance
- **Dark/Light mode** — Toggle with sun/moon icon
- **No hydration errors** — CSS-based theme switching
- **Font size control** — Small / Medium / Large
- **Glass-morphism design** — Beautiful frosted glass UI
- **Neon accents** — Cyan and purple glow effects

### ✨ Animations & Transitions
- **Message slide-in** — User messages from right, AI from left
- **Typing indicator** — Animated bouncing dots while AI thinks
- **Loading skeletons** — Shimmer effect while content loads
- **Hover effects** — Cards lift, sidebar items shift
- **Button glow** — Neon glow on interactive elements
- **Smooth transitions** — Page and component transitions

### 👤 Authentication
- **Email/Password** — Sign up and login
- **OAuth** — Google authentication support
- **Session management** — Secure cookie-based sessions
- **Protected routes** — Middleware redirects unauthenticated users

### ⚙️ Settings Page
- **Profile** — Display name (saved to DB), email (read-only)
- **Appearance** — Theme toggle, font size selector
- **AI Settings** — Model picker, temperature slider
- **AI Memories** — View, add, delete memories
- **Data & Privacy** — Export chats, delete all data, logout
- **About** — App version, tech stack info

---

## 🛠️ Tech Stack

### Frontend
| Technology | Purpose |
|---|---|
| **Next.js 16** | React framework (App Router, Turbopack) |
| **TypeScript** | Type-safe development |
| **Mantine UI v7** | Component library |
| **Zustand** | State management |
| **React Markdown** | Markdown rendering |
| **React Syntax Highlighter** | Code block highlighting |
| **Tabler Icons** | Icon set |
| **react-textarea-autosize** | Auto-expanding textarea |
| **Framer Motion** | Animations (installed) |

### Backend
| Technology | Purpose |
|---|---|
| **Groq Cloud** | AI inference (LLMs + Vision) |
| **Supabase** | Auth, Database (PostgreSQL), RLS |
| **pdf-parse-fork** | Server-side PDF text extraction |
| **mammoth** | DOCX text extraction |

### Code Execution
| Technology | Purpose |
|---|---|
| **Pyodide v0.27** | Python runtime (WebAssembly) loaded from CDN |
| **Browser eval()** | JavaScript execution (sandboxed) |

### AI Models (via Groq — FREE)
| Model | Type |
|---|---|
| `llama-3.3-70b-versatile` | Text (default) |
| `llama-3.1-8b-instant` | Text (fast + memory extraction) |
| `mixtral-8x7b-32768` | Text (long context) |
| `gemma2-9b-it` | Text (efficient) |
| `meta-llama/llama-4-scout-17b-16e-instruct` | Vision (image analysis) |

---

## 📁 Project Structure

```
lumivra-ai/
├── app/
│   ├── (auth)/
│   │   ├── login/page.tsx              # Login page
│   │   └── signup/page.tsx             # Signup page
│   ├── api/
│   │   ├── chat/
│   │   │   ├── route.ts               # Streaming AI endpoint (+ vision + memory)
│   │   │   └── title/route.ts          # Auto-generate chat titles
│   │   ├── memory/
│   │   │   └── extract/route.ts        # AI memory auto-extraction
│   │   ├── parse-pdf/route.ts          # Server-side PDF parsing
│   │   └── auth/callback/route.ts      # OAuth handler
│   ├── chat/
│   │   ├── layout.tsx                  # Chat layout (sidebar + main + font size)
│   │   └── page.tsx                    # Chat page
│   ├── settings/page.tsx               # Settings page (profile, AI, memories)
│   ├── globals.css                     # Global styles + animations
│   ├── layout.tsx                      # Root layout (loads Pyodide script)
│   └── page.tsx                        # Redirects to /login
│
├── components/
│   ├── chat/
│   │   ├── ChatArea.tsx                # Main chat + streaming + edit + files + vision
│   │   ├── MessageBubble.tsx           # Message display + code execution + input modal
│   │   ├── PromptInput.tsx             # Input + file attach + paste + drag-drop
│   │   ├── ChatSkeleton.tsx            # Loading skeleton
│   │   └── TopBar.tsx                  # Theme toggle + settings link
│   └── sidebar/
│       └── Sidebar.tsx                 # Chat list + pin + search + profile
│
├── lib/
│   ├── supabase/
│   │   ├── client.ts                   # Browser Supabase client
│   │   ├── server.ts                   # Server Supabase client
│   │   ├── middleware.ts               # Session handler
│   │   ├── chats.ts                    # Chat/Message DB operations
│   │   ├── settings.ts                 # User settings operations
│   │   └── memories.ts                 # AI memory operations
│   ├── fileParser.ts                   # File parsing (text, PDF, DOCX, images)
│   └── codeRunner.ts                   # 🆕 Code execution (JS + Python) + input detection
│
├── store/
│   └── chatStore.ts                    # Zustand global state
│
├── types/
│   └── index.ts                        # TypeScript interfaces
│
├── theme.ts                            # Mantine theme config
├── proxy.ts                            # Next.js 16 middleware
├── .env.local                          # Environment variables
├── postcss.config.mjs                  # PostCSS config
└── README.md                           # This file
```

---

## 🗄️ Database Schema

### Tables

#### `chats`
| Column | Type | Description |
|---|---|---|
| id | UUID | Primary key |
| user_id | UUID | Foreign key → auth.users |
| title | TEXT | Chat title (auto-generated) |
| icon | TEXT | Emoji icon |
| is_pinned | BOOLEAN | Pin status |
| created_at | TIMESTAMPTZ | Creation time |
| updated_at | TIMESTAMPTZ | Last activity |

#### `messages`
| Column | Type | Description |
|---|---|---|
| id | UUID | Primary key |
| chat_id | UUID | Foreign key → chats |
| role | TEXT | 'user' or 'assistant' |
| content | TEXT | Message text |
| attachments | JSONB | File metadata (name, size) |
| created_at | TIMESTAMPTZ | Creation time |

#### `user_settings`
| Column | Type | Description |
|---|---|---|
| id | UUID | Primary key |
| user_id | UUID | Foreign key → auth.users (unique) |
| display_name | TEXT | User's display name |
| model | TEXT | Selected AI model |
| temperature | FLOAT | AI creativity (0-2) |
| system_prompt | TEXT | System prompt (reserved) |
| font_size | TEXT | 'small' / 'medium' / 'large' |
| created_at | TIMESTAMPTZ | Creation time |
| updated_at | TIMESTAMPTZ | Last update |

#### `user_memories`
| Column | Type | Description |
|---|---|---|
| id | UUID | Primary key |
| user_id | UUID | Foreign key → auth.users |
| content | TEXT | Memory fact |
| created_at | TIMESTAMPTZ | Creation time |

### Row Level Security (RLS)
All tables have RLS enabled. Users can only access their own data.

---

## 🚀 Getting Started

### Prerequisites
- Node.js 18+
- pnpm (or npm/yarn)
- Supabase account
- Groq Cloud account

### 1. Clone the repo
```bash
git clone https://github.com/yourusername/lumivra-ai.git
cd lumivra-ai
```

### 2. Install dependencies
```bash
pnpm install
```

### 3. Set up environment variables
Create `.env.local`:
```env
# Supabase
NEXT_PUBLIC_SUPABASE_URL=your_supabase_url
NEXT_PUBLIC_SUPABASE_ANON_KEY=your_supabase_anon_key

# Groq
GROQ_API_KEY=your_groq_api_key
```

### 4. Set up Supabase database
Run these SQL queries in Supabase SQL Editor:

```sql
-- Chats table
CREATE TABLE chats (
  id UUID DEFAULT gen_random_uuid() PRIMARY KEY,
  user_id UUID REFERENCES auth.users(id) ON DELETE CASCADE,
  title TEXT DEFAULT 'New Chat',
  icon TEXT DEFAULT '💬',
  is_pinned BOOLEAN DEFAULT FALSE,
  created_at TIMESTAMPTZ DEFAULT NOW(),
  updated_at TIMESTAMPTZ DEFAULT NOW()
);

-- Messages table
CREATE TABLE messages (
  id UUID DEFAULT gen_random_uuid() PRIMARY KEY,
  chat_id UUID REFERENCES chats(id) ON DELETE CASCADE,
  role TEXT NOT NULL CHECK (role IN ('user', 'assistant')),
  content TEXT NOT NULL,
  attachments JSONB DEFAULT NULL,
  created_at TIMESTAMPTZ DEFAULT NOW()
);

-- User settings table
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

-- User memories table
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

-- Enable RLS on all tables
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

### 5. Run the development server
```bash
pnpm dev
```

Open [http://localhost:3000](http://localhost:3000)

---

## 🧪 Try It Out

### Test Code Execution
Ask the AI:
```
Write Python code that takes user's name and age as input then prints "Hello [name], you are [age] years old"
```
1. Click the green ▶ Run button on the code block
2. Input modal pops up asking for name and age
3. Fill in values → click Run
4. See output below the code

### Test Image Understanding
1. Take a screenshot of any error
2. Paste (Cmd+V) into chat
3. Ask "What's this error about?"
4. AI analyzes the image

### Test AI Memory
1. Tell AI: "My name is Gautham and I prefer Python"
2. Go to Settings → AI Memories → see auto-extracted facts
3. Start a new chat → ask "What's my name?"
4. AI remembers!

### Test File Upload
- Drag a PDF onto the input area
- Or click 📎 to pick a file
- Or paste an image with Cmd+V
- Ask AI to analyze it

---

## 🔒 Security

- ✅ **Row Level Security (RLS)** — Users can only access own data
- ✅ **Server-side API keys** — Groq API key never exposed to client
- ✅ **Model validation** — Prevents injection via model parameter
- ✅ **Temperature clamping** — Restricted to 0-2 range
- ✅ **System prompt hardcoded** — Cannot be modified by users
- ✅ **File size limits** — Max 5MB (4MB for images)
- ✅ **Auth middleware** — Protected routes redirect to login
- ✅ **Session cookies** — Secure, HttpOnly
- ✅ **Code execution sandboxed** — JS runs in browser context, Python in WASM

---

## 📦 Key Dependencies

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
  "mammoth": "^1.x",
  "framer-motion": "^11.x"
}
```

**External (loaded via CDN):**
- `pyodide@0.27.5` — Python runtime for in-browser code execution

---

## 🗺️ Roadmap

### ✅ Completed
- [x] Chat with AI (streaming)
- [x] Stop generation
- [x] Edit messages & regenerate
- [x] File attachments (code, PDF, DOCX, text, data)
- [x] Image understanding (Groq Vision)
- [x] AI Memory (auto-extract + manual)
- [x] Dark/Light mode
- [x] Pin chats
- [x] Settings page (model, temperature, font size)
- [x] Animations & transitions
- [x] Export chats (JSON)
- [x] Delete all data
- [x] Paste & drag-drop files
- [x] **Code execution (JavaScript + Python)** ⚡
- [x] **Interactive input modal for code execution** 📥

### 🔜 Planned
- [ ] Voice input (browser Speech API)
- [ ] Deploy to Vercel
- [ ] Share chat via public link
- [ ] Export single chat as PDF/Markdown
- [ ] Keyboard shortcuts (Cmd+K, etc.)
- [ ] Search inside messages
- [ ] Mobile-responsive polish
- [ ] Token usage tracking
- [ ] Code theme picker
- [ ] Support more languages in code execution (HTML preview, SQL, etc.)

---

## 🤝 Contributing

1. Fork the project
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

---

## 📄 License

This project is licensed under the MIT License.

---

## 👤 Author

**Gautham Jayesh**
- GitHub: [@yourusername](https://github.com/yourusername)
- LinkedIn: [Gautham Jayesh](https://linkedin.com/in/yourprofile)
- Email: gautham.xc@gmail.com

---

## 🙏 Acknowledgments

- [Groq](https://groq.com) — Lightning-fast AI inference
- [Supabase](https://supabase.com) — Backend-as-a-Service
- [Mantine](https://mantine.dev) — Beautiful React components
- [Next.js](https://nextjs.org) — React framework
- [Pyodide](https://pyodide.org) — Python in the browser
- [Vercel](https://vercel.com) — Deployment platform

---

<div align="center">

### 🚀 DEVELOPED BY GAUTHAM JAYESH 🚀

**Next.js 16 • TypeScript • Supabase • Groq Cloud • Mantine UI • Pyodide**

## License

Copyright © 2026 Gautham Jayesh.

This repository is published for portfolio and demonstration purposes only.

Lumivra AI is a personal project published to showcase my software engineering, AI integration, and full-stack development skills. The source code is not open source and may not be copied, modified, redistributed, or used without permission.

</div>
