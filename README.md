<div align="center">

# ⚡ DENZIE
### Supreme AI Architecture — ALPHA

**A futuristic, multimodal AI interface powered by Google Gemini**

![Version](https://img.shields.io/badge/version-4.2.0--stable-blue?style=for-the-badge)
![React](https://img.shields.io/badge/React-19-61DAFB?style=for-the-badge&logo=react)
![TypeScript](https://img.shields.io/badge/TypeScript-5.8-3178C6?style=for-the-badge&logo=typescript)
![Vite](https://img.shields.io/badge/Vite-6-646CFF?style=for-the-badge&logo=vite)

</div>

---

## Overview

DENZIE is a feature-rich, visually immersive AI chat interface built on Google Gemini. It supports text, voice, images, live camera feeds, and multiple AI personas — all wrapped in a highly customizable, dark-themed UI.

---

## Features

### 🤖 AI & Models
- **Multi-model switching** — Gemini Flash Lite, Flash (Pro), and Pro (Ultra) with Thinking mode
- **AI Personas** — Oracle, Architect, Renegade, System-X, each with distinct personalities
- **Streaming responses** — Real-time token-by-token output
- **Memory extraction** — Automatically distills important info from conversations

### 🎨 Themes
| Theme | Description |
|-------|-------------|
| **Denzie (God)** | Clean, dark, authoritative — the default production look |
| **Cosmic Futurist** | Deep space aesthetic with cyan accents |
| **Obsidian** | Warm, dark, and professional |
| **Ethereal** | Light, airy, minimal |
| **Cyberpunk** | Neon-lit and high contrast |
| **Custom** | Define your own colors and style |

### 🎙️ Voice & Audio
- **Voice input** — Speak your messages with speech-to-text
- **Text-to-speech** — Gemini TTS or native browser TTS
- **Auto-read** — Responses read aloud automatically
- **Ambient sounds** — Rain, forest, or cyberpunk background audio
- **Voice note attachments** — Record and send audio clips

### 📎 Multimodal Input
- **Image attachments** — Upload and analyze images
- **Visual analysis** — AI describes and reasons about uploaded images
- **Live camera mode** — Real-time video feed analysis via `LiveDashboard`
- **Audio attachments** — Send voice recordings alongside text

### 🌍 Internationalization
Supports 12 languages for input and output:
English, Spanish, French, German, Italian, Portuguese, Japanese, Chinese, Korean, Russian, Hindi, Arabic

### ⚙️ Customization
- Light / Dark / System theme mode
- Text zoom control
- Custom input bar styling (background, border, glow color)
- Custom AI instructions per session
- User name and avatar

---

## Getting Started

### Prerequisites
- [Node.js](https://nodejs.org/) v18 or higher
- A [Google Gemini API key](https://aistudio.google.com/app/apikey)

### Installation

```bash
# 1. Clone the repo
git clone https://github.com/YOUR_USERNAME/denzie.git
cd denzie

# 2. Install dependencies
npm install

# 3. Add your Gemini API key
echo "GEMINI_API_KEY=your_key_here" > .env.local

# 4. Start the dev server
npm run dev
```

Open [http://localhost:5173](http://localhost:5173) in your browser.

### Build for Production

```bash
npm run build
npm run preview
```

---

## Project Structure

```
denzie/
├── components/
│   ├── ChatMessage.tsx       # Message bubbles with reactions & suggestions
│   ├── InputBar.tsx          # Rich input (voice, image, file, text)
│   ├── LiveDashboard.tsx     # Live camera feed + AI analysis
│   ├── NeuralAvatar.tsx      # Animated neural face component
│   ├── Orb.tsx               # Animated orb avatar
│   ├── ParticleFace.tsx      # Particle-based face animation
│   ├── ReactiveBackground.tsx # Dynamic animated background
│   ├── SettingsModal.tsx     # Full settings panel
│   ├── Sidebar.tsx           # Conversation history
│   └── WelcomeScreen.tsx     # Onboarding / init screen
├── services/
│   ├── audio.ts              # Audio playback utilities
│   ├── geminiService.ts      # Gemini API (streaming, TTS, memory)
│   ├── themeConfig.ts        # Theme & template definitions
│   └── themeExtractor.ts     # Dynamic theme generation
├── App.tsx                   # Main app shell & state
├── types.ts                  # TypeScript types & enums
└── index.tsx                 # Entry point
```

---

## Environment Variables

| Variable | Description |
|----------|-------------|
| `GEMINI_API_KEY` | Your Google Gemini API key (required) |

> ⚠️ Never commit your `.env.local` file. It is already listed in `.gitignore`.

---

## Tech Stack

- **React 19** + **TypeScript 5.8**
- **Vite 6** — build tooling
- **Tailwind CSS** — utility-first styling
- **Google Gemini API** (`@google/genai`) — AI backbone
- **Lucide React** — icons

---

## License

This project is private. All rights reserved.

---

<div align="center">
  <sub>Built with ⚡ by the DENZIE team</sub>
</div>
