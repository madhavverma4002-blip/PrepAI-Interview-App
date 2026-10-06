# PrepAI — AI Interviewer for Every Field 🤖🎙️

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
[![PWA Ready](https://img.shields.io/badge/PWA-Ready-emerald.svg)](https://developer.mozilla.org/en-US/docs/Web/Progressive_web_apps)
[![Web Speech API](https://img.shields.io/badge/Speech%20AI-Voice%20%26%20STT-purple.svg)](https://developer.mozilla.org/en-US/docs/Web/API/Web_Speech_API)

> **PrepAI** is a state-of-the-art, interactive AI-powered job interview practice platform supporting **every professional field and custom job title**. Practice mock interviews with natural AI voice synthesis, live microphone speech recognition, dynamic audio spectrum visualizers, filler-word detection, real-time WPM metrics, and deep post-interview score analytics.

---

## 🌟 Key Features

- **🌐 Every Career Field Supported**: Pre-built domains (Software Engineering, Data Science, Product Management, Finance, Marketing, Healthcare, HR, Civil Engineering) + **Universal Custom Role Generator** for any job title (e.g. *Quantum Computing Specialist*, *Pilot*, *Dental Assistant*).
- **🎙️ Speech Synthesis (AI Voice)**: Interactive AI Interviewer persona with customizable system voice, speech speed rate, and pitch controls.
- **🗣️ Real-Time Speech Recognition (STT)**: Speaks responses naturally into the microphone with live transcript streaming, words-per-minute (WPM) tracking, and filler-word detection (*"um"*, *"uh"*, *"like"*, *"you know"*).
- **📊 Canvas Audio Spectrum Visualizer**: HTML5 Canvas rendering dynamic audio frequency bars during voice responses.
- **📷 Mirrored Webcam Preview**: Optional live video feed to practice body language and facial expression delivery.
- **⚡ Dual AI Evaluation Engine**:
  - **Local Heuristic NLP Engine**: Evaluates Technical Coverage, STAR Framework alignment, Communication Clarity, Problem Solving, and Delivery WPM (runs 100% offline).
  - **Google Gemini API Integration**: Optional API key setting for generative LLM feedback and custom model answers.
- **📱 Native PWA & Mobile App Ready**: Progressive Web App with standalone installability, offline Service Worker caching, and Capacitor mobile build configuration.

---

## 🚀 Quick Start & Installation

```bash
# Clone the repository
git clone https://github.com/madhavverma4002-blip/PrepAI-Interview-App.git
cd PrepAI-Interview-App

# Start local server with Python
python3 -m http.server 8085

# Open http://localhost:8085 in your browser
```

---

## 📤 Push Code to GitHub

Run these commands in your Terminal to push your codebase to GitHub:

```bash
git remote add origin https://github.com/madhavverma4002-blip/PrepAI-Interview-App.git
git branch -M main
git push -u origin main
```

---

## 📂 Project Architecture

```
PrepAI/
├── index.html              # Main Single Page Application UI
├── styles.css              # Ultra-premium Dark Theme Glassmorphism stylesheet
├── manifest.json           # Web App Manifest for PWA installation
├── sw.js                   # Service Worker for offline PWA caching
├── capacitor.config.json   # Native mobile app configuration (Capacitor)
├── js/
│   ├── questionsData.js    # Pre-built question bank & custom role generator
│   ├── speechEngine.js     # SpeechSynthesis, SpeechRecognition, & Canvas Visualizer
│   ├── evaluationEngine.js # Heuristic NLP Evaluator & Gemini API integration
│   └── app.js              # State manager, navigation router, & camera controller
├── icons/                  # High-resolution PWA icons (192x192, 512x512)
└── images/                 # App background and avatar graphic assets
```

---

## 🛠️ Technology Stack

- **Frontend**: HTML5, Vanilla CSS3 (Glassmorphism, CSS Custom Properties), JavaScript (ES6+).
- **UI Framework**: Tailwind CSS (CDN), Lucide Icons.
- **Audio & Speech**: Web Speech API (`SpeechSynthesis` & `SpeechRecognition`), Web Audio API (`AudioContext`, `AnalyserNode`).
- **Visuals**: HTML5 `<canvas>` rendering engine.
- **Storage**: `localStorage` API for history and configuration persistence.
- **PWA**: Web App Manifest & Service Worker.

---

## 📜 License

This project is licensed under the [MIT License](LICENSE).
