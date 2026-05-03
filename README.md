# 🧠 GROOT OS v2.1_ALPHA

> **Neural Interface AI Assistant**

GROOT OS is a high-fidelity, voice-reactive AI interface designed with a focus on immersive aesthetics and low-latency interaction. It features multiple personality profiles, real-time 3D visualization, and a sophisticated HUD (Heads-Up Display) layout inspired by cyberpunk and sci-fi aesthetics.

---

## ✨ Core Features

- **🎭 Multi-Persona Integration**: Switch between three distinct AI personalities:
  - **LISA**: Sweet, caring, and supportive companion.
  - **ATLAS**: Cold, calculating cyberpunk AI sentinel.
  - **NOVA**: Aggressive, direct tactical AI.
- **🌐 Real-time Voice Interaction**: 
  - Integrated **Wake Word** detection ("Hey Lisa").
  - **VAD (Voice Activity Detection)** for hands-free auto-listening.
  - Real-time **Streaming Speech-to-Text** and **Text-to-Speech**.
- **🌀 3D Neural Visualization**: A custom-built **Mathematical Fibonacci Sphere** that reacts dynamically to the AI's voice frequency data.
- **🖥️ Immersive UI/UX**:
  - **Matrix Rain Background**: Subtle emerald digital cascade.
  - **CRT Scanlines**: Authentic retro-tech visual filter.
  - **Terminal Logs**: Real-time hacker-style system diagnostics.
  - **Boot Sequence**: Cyberpunk-style kernel initialization on startup.

## 🛠️ Tech Stack

- **Framework**: [React 19](https://react.dev/) + [Vite](https://vitejs.dev/)
- **Icons**: [Lucide React](https://lucide.dev/)
- **State Management**: React Hooks (Ref-heavy for low-latency audio handling)
- **Communication**: WebSockets (Real-time duplex streaming)
- **Visuals**: HTML5 Canvas (3D Math Sphere & Matrix Background)

## 🚀 Getting Started

### Prerequisites
- Node.js (v18+)
- npm / yarn

### Installation
1. Clone the repository.
2. Navigate to the `frontend` directory:
   ```bash
   cd frontend
   ```
3. Install dependencies:
   ```bash
   npm install
   ```
4. Start the development server:
   ```bash
   npm run dev
   ```

### ⚠️ Security Notice (Microphone Access)
Mobile browsers require a **secure HTTPS connection** to access the microphone. For local testing on mobile devices, use an HTTPS tunnel like **Ngrok** or deploy to a secure host like **Vercel/Netlify**.

## 🔧 Configuration

The frontend looks for a WebSocket URL in the environment variables:
`VITE_WS_URL=ws://your-backend-ip:8000/ws/chat`

If not provided, it defaults to the current hostname on port 8000.

---

*Designed for the future of human-AI interaction.*

