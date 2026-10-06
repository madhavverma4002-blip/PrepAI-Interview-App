# 📊 PrepAI - Complete Project Presentation (PPT Outline & Speaker Notes)

> Use this presentation guide to explain **PrepAI** to professors, recruiters, judges, investors, or team members!

---

## 📌 Slide 1: Title Slide

### **Title**: PrepAI — AI-Powered Interviewer Platform for Every Field
- **Subtitle**: Interactive Speech AI, Real-time Voice Evaluation, and Post-Interview Performance Analytics
- **Presented By**: [Your Name / Team Name]
- **Key Highlight**: Supports **Any Career Domain** + Custom Job Role Generator

---

## 📌 Slide 2: Problem Statement & Motivation

### **The Problem**:
1. **Interview Anxiety & Lack of Practice**: Over 75% of job candidates suffer from severe interview anxiety due to inadequate real-world mock interview practice.
2. **Expensive Coaching**: Personal interview coaches and specialized bootcamps cost hundreds of dollars per session.
3. **Generic Question Banks**: Most existing practice apps only provide generic static software engineering questions, ignoring domains like Healthcare, Finance, Marketing, HR, or niche engineering fields.
4. **No Real-Time Speech Feedback**: Reading answers on paper doesn't evaluate speaking cadence, filler-word usage (*"um"*, *"uh"*), or verbal confidence.

### **Our Solution (PrepAI)**:
- An **on-demand, interactive AI interviewer** accessible 24/7 on web and mobile.
- Speaks questions aloud, listens to candidate responses via speech-to-text, tracks WPM and filler words, and delivers deep analytical evaluations.

---

## 📌 Slide 3: Key Features & Value Proposition

| Feature | Description |
| :--- | :--- |
| **🌐 Every Field Support** | 8+ pre-built career domains + **Procedural Custom Role Generator** for any job title. |
| **🎙️ Voice Speech AI** | Natural AI voice output (`SpeechSynthesis`) with customizable voice persona, speed, and pitch. |
| **🗣️ Real-Time STT & Metrics** | Speech-to-text input (`SpeechRecognition`), WPM counter, and filler-word detection. |
| **📊 Canvas Spectrum Visualizer** | Dynamic glowing audio visualizer matching microphone speech intensity. |
| **📷 Video Feed Overlay** | Mirrored webcam preview box for body language and eye contact practice. |
| **🧠 Dual Evaluation Engine** | Built-in offline NLP heuristic evaluator + optional Google Gemini LLM API integration. |
| **📱 Native PWA App Form** | 1-click installation on desktop/mobile + offline Service Worker caching. |

---

## 📌 Slide 4: System Architecture & Workflow

```
+-------------------------------------------------------------+
| 1. User Selects Domain or Types Custom Role                 |
+-------------------------------------------------------------+
                              │
                              ▼
+-------------------------------------------------------------+
| 2. Configure Parameters (Level, Question Count, Voice, Mic) |
+-------------------------------------------------------------+
                              │
                              ▼
+-------------------------------------------------------------+
| 3. PrepAI Question Generator / Dynamic Bank                 |
+-------------------------------------------------------------+
                              │
                              ▼
+-------------------------------------------------------------+
| 4. Live Chamber: AI Voice Speaks Question Aloud             |
+-------------------------------------------------------------+
                              │
                              ▼
+-------------------------------------------------------------+
| 5. Candidate Answers via Microphone (Speech Recognition)    |
+-------------------------------------------------------------+
                              │
                              ▼
+-------------------------------------------------------------+
| 6. Speech Engine Tracks Transcript, WPM & Filler Words      |
+-------------------------------------------------------------+
                              │
                              ▼
+-------------------------------------------------------------+
| 7. Evaluation Engine: Technical, STAR, Clarity, Delivery    |
+-------------------------------------------------------------+
                              │
                              ▼
+-------------------------------------------------------------+
| 8. Post-Interview Score Analytics Dashboard                 |
+-------------------------------------------------------------+
```

---

## 📌 Slide 5: Deep Dive — Speech AI & Audio Engine

- **Voice Synthesis (TTS)**:
  - Uses browser native `SpeechSynthesisUtterance`.
  - Dynamically discovers system voices (e.g., Google US Female, Samantha, Alex, Karen, Victoria).
  - Allows full speed rate adjustment (`0.75x` to `1.4x`) and pitch tuning (`0.8x` to `1.2x`).
  - Includes instant **"Test Voice Sound"** audio preview button.
- **Speech Recognition (STT)**:
  - Utilizes `SpeechRecognition` / `webkitSpeechRecognition`.
  - Supports continuous interim transcript streaming.
  - Natural Language filler word detector searching for: *"um"*, *"uh"*, *"like"*, *"you know"*, *"basically"*, *"literally"*, *"honestly"*.
  - Live Words-Per-Minute (WPM) calculation engine.

---

## 📌 Slide 6: Deep Dive — Evaluation & Scoring Algorithm

Each response is evaluated across **4 weighted categories (0-100 score)**:

1. **Technical Coverage (35%)**: Keyword density matching against domain-specific technical terminology.
2. **Communication & Structure (25%)**: Detection of STAR Method markers (*Situation, Task, Action, Result, Outcome*) minus filler-word penalties.
3. **Problem Solving & Depth (25%)**: Analytical breakdown, length, and logical structure.
4. **Delivery & Pace (15%)**: Optimal speaking rate (ideal: 110–160 WPM) and voice clarity.

**Overall Verdict Rating**:
- **88 - 100**: *Strong Hire (Outstanding)*
- **75 - 87**: *Hire (Proficient)*
- **60 - 74**: *Passable (Needs Polish)*
- **Below 60**: *Needs Improvement*

---

## 📌 Slide 7: UI/UX & Design System

- **Glassmorphism Aesthetics**: Modern dark theme background (`#070a12`), backdrop-blur cards, and radial ambient glowing blobs.
- **Micro-Animations**: Breathing pulse indicators on the AI Avatar when speaking or listening.
- **Typography**: Google Fonts (`Plus Jakarta Sans` for headers, `Outfit` for body text).
- **Responsive Layout**: Desktop grid layout + Mobile bottom navigation dock.

---

## 📌 Slide 8: Technical Demonstration (Step-by-Step Flow)

1. **Step 1: Role Selection**: Choose a featured category or enter a custom title (e.g. *"Aerospace Engineer"*).
2. **Step 2: Setup**: Pick difficulty level, question count, and test AI voice sound.
3. **Step 3: Interview Chamber**: AI speaks question aloud ➔ Candidate clicks microphone ➔ Canvas audio spectrum pulses ➔ Transcript streams in real-time.
4. **Step 4: Submission**: Answer evaluated instantly.
5. **Step 5: Score Report**: Comprehensive dashboard displaying overall score, 4 sub-score bars, strengths, areas for improvement, and ideal model answers.

---

## 📌 Slide 9: Future Scope & Enhancement Roadmap

- [ ] **Multi-Lingual Voice Support**: Expand full voice interaction in Hindi, Spanish, French, and German.
- [ ] **AI Facial Expression Analysis**: Computer Vision emotion tracking using WebRTC camera stream.
- [ ] **Resume / CV Parsing**: Upload candidate PDF resume to generate hyper-personalized resume-based questions.
- [ ] **Real-Time Peer Mock Interviews**: WebSockets multiplayer mock interviews with live peer evaluation.

---

## 📌 Slide 10: Conclusion & Q&A

- **Summary**: PrepAI is a complete, scalable, zero-dependency AI interviewing platform bridging the gap between practice and hiring success.
- **GitHub Repository**: Ready for GitHub upload with `README.md`, `.gitignore`, and `manifest.json`.
- **Live Server**: `http://localhost:8085`

**Thank You! Questions & Discussion.**
