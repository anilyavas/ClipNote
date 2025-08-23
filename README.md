# 📝 ClipNote — AI-Powered Smart Notes App

ClipNote is an **AI-assisted mobile app** built with **React Native** that helps users manage and organize short notes, audio snippets, and quick thoughts effortlessly.  
It’s designed for solo developers as a **portfolio-worthy project** while being practical for real-world use.

---

## ✨ Features

- 🖊️ **Quick Notes** — Create, edit, and delete text notes easily.  
- 🎙️ **Voice Notes with Transcription** — Record audio and convert it into searchable text (powered by AI).  
- 🤖 **AI Summaries** — Summarize long notes into concise points.  
- 🧩 **Smart Categorization** — AI auto-tags notes (e.g., "work," "study," "personal").  
- 🔍 **Search & Filter** — Full-text search with category filtering.  
- 📱 **Offline-First** — Notes stored locally and synced to cloud (Supabase).  
- ☁️ **Cloud Sync** — Access notes across devices with Supabase authentication & database.  
- 🔒 **Authentication** — Email & password login using Supabase.  

---

## 🛠️ Tech Stack

- **React Native (Expo)** — Cross-platform app development  
- **TypeScript** — Type safety and better DX  
- **Supabase** — Authentication & database (PostgreSQL)  
- **OpenAI API** — For transcription, summaries, and tagging  
- **Lottie** — Smooth animations for loading states  
- **FlashList** — High-performance list rendering  
- **Tailwind CSS (NativeWind)** — Styling  

---

## 📂 Project Structure

```bash
clipnote/
├── app/                  # Expo Router pages
│   ├── index.tsx         # Home screen (list of notes)
│   ├── note/[id].tsx     # Single note details
│   ├── new-note.tsx      # Create new note
│   ├── auth/             # Auth screens (login/register)
│
├── components/           # Reusable UI components
│   ├── NoteCard.tsx
│   ├── AudioRecorder.tsx
│   ├── AIButton.tsx
│
├── lib/                  # Config & setup
│   ├── supabase.ts       # Supabase client
│   ├── openai.ts         # OpenAI client
│
├── utils/                # Helper functions
│   ├── formatDate.ts
│   ├── audioHelpers.ts
│
├── hooks/                # Custom hooks
│   ├── useAuth.ts
│   ├── useNotes.ts
│
├── assets/               # Images, Lottie files
│
├── package.json
├── tsconfig.json
└── README.md
