# B.A.D.D.I.E.

**Behavioural Architectures for Digitally-Defined Independent Entities**

A local-first desktop AI companion with personality modelling, RAG-based long-term memory, real-time voice interaction, machine vision, and an animated Live2D avatar.

## Overview

B.A.D.D.I.E. is a privacy-first AI companion that runs entirely on your desktop. Unlike cloud-based assistants, all data stays on your device — conversations, memories, and personality configurations never leave your hardware.

### Key Features

- 🧠 **Personality Engine** — Configurable "baddie" persona with adaptive behaviour
- 💾 **Long-Term Memory** — RAG-based typed memory (episodic, semantic, procedural)
- 🎙️ **Voice Interaction** — Local Whisper STT + neural TTS with streaming
- 👁️ **Machine Vision** — Screen capture and camera input for environmental awareness
- 🎭 **Live2D Avatar** — Animated 2D avatar with lip-sync and expression mapping
- 🔒 **Local-First** — All data stays on your device

## Architecture

All system diagrams are written in **Mermaid** format (`.mmd` files in `figures/`). Render them with:

```bash
mmdc -i figures/architecture.mmd -o figures/architecture.pdf
mmdc -i figures/personality-pipeline.mmd -o figures/personality-pipeline.pdf
mmdc -i figures/voice-pipeline.mmd -o figures/voice-pipeline.pdf
mmdc -i figures/memory-architecture.mmd -o figures/memory-architecture.pdf
```

### System Architecture
![System Architecture](figures/architecture.mmd)

### Personality Pipeline
![Personality Pipeline](figures/personality-pipeline.mmd)

### Voice Pipeline
![Voice Pipeline](figures/voice-pipeline.mmd)

### Memory Architecture
![Memory Architecture](figures/memory-architecture.mmd)

## Tech Stack

| Component | Technology |
|-----------|-----------|
| Desktop Shell | Tauri 2.0 (Rust + WebView) |
| Frontend | Svelte 5 + TypeScript |
| LLM | Gemini 3.1 Flash Lite |
| STT | faster-whisper (local) |
| TTS | Piper / Kokoro (local) |
| VAD | Silero VAD |
| RAG | LanceDB (local vector store) |
| Avatar | Live2D Cubism SDK + WebGL |
| Memory | LanceDB + SQLite |

## Research Paper

The full academic paper (ACM format, APA 7th edition) is available in this repository:

- [`main.tex`](main.tex) — LaTeX source
- [`references.bib`](references.bib) — Bibliography

## Author

**Amir Hafizi Bin Musa**  
Student ID: 2024745815  
Universiti Teknologi MARA (UiTM) Perak, Tapah Campus, Malaysia  
Email: amirhafizi443@gmail.com

## License

MIT License — see [LICENSE](LICENSE) for details.
