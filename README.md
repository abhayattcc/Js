# 📖 GK by Abhaya — Odia GK & Grammar Study App

> **A free, offline-capable Progressive Web App (PWA) for Odia & English General Knowledge, Lucent GK Mock Tests, Odia Grammar, and bilingual dictionary — built for competitive exam aspirants.**

<div align="center">

[![Live App](https://img.shields.io/badge/🚀%20Open%20Live%20App-4CAF50?style=for-the-badge&logo=googlechrome&logoColor=white)](https://abhayattcc.github.io/abhayagk/)
[![PWA](https://img.shields.io/badge/PWA-Offline%20Ready-blue?style=for-the-badge&logo=pwa&logoColor=white)](https://abhayattcc.github.io/abhayagk/)
[![License](https://img.shields.io/badge/License-Free%20to%20Use-orange?style=for-the-badge)](https://abhayattcc.github.io/abhayagk/)
[![Language](https://img.shields.io/badge/Language-Odia%20%7C%20English-red?style=for-the-badge)](https://abhayattcc.github.io/abhayagk/)

</div>

---

## 🌐 Live Demo

**👉 [https://abhayattcc.github.io/abhayagk/](https://abhayattcc.github.io/abhayagk/)**

Open it in any browser — no installation required. Works on mobile and desktop.

---

## 📌 About the App

**GK by Abhaya** is a comprehensive, bilingual (Odia + English) study platform designed for students preparing for OPSC, OSSSC, Railway, SSC, and other competitive exams. It combines a rich GK content library, interactive MCQ mock tests, an Odia/Hindi dictionary, Text-to-Speech reading, PDF support, and an interactive Mind Map viewer — all in a single, lightweight Progressive Web App that works even without an internet connection.

---

## ✨ Features

### 📚 Content Library

- **Odisha GK Mock Test** — Chapter-wise MCQ practice covering Odisha-specific General Knowledge
- **Lucent GK Theory (English)** — Full theoretical coverage of Lucent GK in English
- **Lucent GK Mock Tests (English)** — Chapter-wise MCQ mock tests in English across:
  - Biology · Chemistry · Economics · History · Geography · Physics · Polity · Static GK
- **Odia GK Theory** — Lucent GK content in ଓଡ଼ିଆ (Odia script)
- **Odia Lucent GK Mock Tests** — Full chapter-wise MCQ tests in Odia:
  - ଜୀବ ବିଜ୍ଞାନ · ରସାୟନ ବିଜ୍ଞାନ · ଅର୍ଥନୀତି · ଇତିହାସ · ଭୂଗୋଳ · ଭୌତିକ ବିଜ୍ଞାନ · ରାଜନୀତି ବିଜ୍ଞାନ · Statik GK
- **English Grammar** — Concepts covering all major grammar topics (Nouns, Verbs, Tenses, Sentences, etc.)
- **Computer Topics** — Computer GK for competitive exams
- **ଓଡ଼ିଆ ବ୍ୟାକରଣ (Odia Grammar)** — 13 structured chapters including ଭାଷା, ଶବ୍ଦ ଗଠନ, ବାକ୍ୟ, ସନ୍ଧି, ପ୍ରତ୍ୟୟ, ସମାସ, ଛନ୍ଦ, ଅଳଙ୍କାର, and more

---

### 🧪 Interactive MCQ Mock Tests

- Auto-parsed Multiple Choice Questions from text content
- Tap-to-select option buttons with **instant right/wrong feedback**
- **Skip button** to move past difficult questions
- Correct answer revealed on skip or wrong attempt
- Batched question sets with **score tracking** (attempted / correct)
- Seamless navigation between question batches

---

### 🗣️ Text-to-Speech (TTS) Reader

- Full **read-aloud** functionality for any content
- Tap any sentence to **start reading from that point**
- **Sentence-level highlighting** as speech progresses
- Supports **Odia**, **Hindi**, and **English** voice selection
- **Pause / Resume / Stop** controls
- Smart voice detection — automatically picks the best available system voice per language

---

### 📖 Bilingual Dictionary Popup

- **Tap any word** while reading to get an instant dictionary popup
- Powered by a compressed SQLite database (`.db.gz`) loaded locally via sql.js
- Supports **English → Odia** and **English → Hindi** lookups
- Displays word meanings, images (where available), and suggestions
- **Search bar** inside the popup for manual word lookup
- Speak button to **pronounce** the dictionary result aloud
- Image delete/restore controls for clean reading

---

### 🗺️ Interactive Mind Map Viewer

- Automatically detects mind map HTML files (structured `<h1>` + `<ul>` format)
- Renders collapsible, color-coded hierarchical trees with up to **5 nesting levels**
- Per-node **expand/collapse** with animated transitions
- **Collapse All / Expand All** global controls
- Notes/explanations displayed per node via `<pre>` blocks
- Level-specific color coding for instant visual depth recognition

---

### 📂 Custom File Upload & Reader

- Upload and read your own `.pdf`, `.txt`, or `.html` files directly in the app
- **PDF support** via PDF.js — extracts text from multi-page PDFs for reading and MCQ parsing
- **TXT file reader** — auto-detects subject-grouped content or MCQ format
- **HTML file viewer** — renders HTML files as rich content or mind maps
- Multi-file upload support — load multiple files at once and read them sequentially

---

### 📶 Offline / PWA Support

- Fully **Progressive Web App (PWA)** — installable to home screen on Android, iOS, and desktop
- **Service Worker** caches all chapter content, fonts, scripts, and databases on first load
- Works completely **offline** after initial cache — no internet needed for revisits
- Cache-first strategy for fast load times

---

### 💾 Reading Position Memory

- Automatically **remembers where you left off** per chapter or uploaded file using `localStorage`
- Returns you to the exact sentence on next visit
- Highlights last-read chapter in the chapter grid when returning to home

---

### 🎨 UI & UX Highlights

- Clean, mobile-first responsive design optimized for small screens
- Noto Sans font with full **Odia script support**
- Smooth animated chapter cards with hover effects
- Full-screen reader mode with dedicated top bar and TTS controls bar
- Progress bar overlay during file loading and database initialization
- Floating **Donate button** (Razorpay) for supporting the developer

---

## 🛠️ Tech Stack

| Technology | Purpose |
|---|---|
| Vanilla HTML / CSS / JavaScript | Core app — no framework dependencies |
| [PDF.js](https://mozilla.github.io/pdf.js/) `v2.14` | PDF text extraction |
| [sql.js](https://github.com/sql-js/sql.js/) `v1.8` | In-browser SQLite for dictionary |
| [pako](https://github.com/nodeca/pako) `v2.0` | Gzip decompression for `.db.gz` dictionary files |
| Web Speech API | Text-to-Speech across Odia, Hindi, English |
| Service Worker + Cache API | PWA offline support |
| localStorage | Reading position persistence |
| GitHub Pages | Free static hosting |

---

## 📁 Repository Structure

```
abhayagk/
├── index.html          # Main PWA app
├── manifest.json       # PWA manifest (icons, theme, name)
├── service-worker.js   # Offline caching logic
├── icon-192.png        # App icon
└── ...
```

Content (chapters, MCQs, grammar) is hosted separately in the [`lucentgkonline`](https://github.com/abhayattcc/lucentgkonline) branch and loaded dynamically.

Dictionary databases are hosted in the [`Best-odia-dictionary`](https://github.com/abhayattcc/Best-odia-dictionary) repository.

---

## 🚀 Getting Started

### Use Online (Recommended)

Simply open: **[https://abhayattcc.github.io/abhayagk/](https://abhayattcc.github.io/abhayagk/)**

### Install as App (PWA)

**Android (Chrome):** Tap the browser menu → "Add to Home Screen"  
**iOS (Safari):** Tap Share → "Add to Home Screen"  
**Desktop (Chrome/Edge):** Click the install icon in the address bar

### Run Locally

```bash
git clone https://github.com/abhayattcc/abhayagk.git
cd abhayagk
# Open index.html with a local server (required for Service Worker)
npx serve .
# or
python -m http.server 8080
```

> ⚠️ Opening `index.html` directly via `file://` disables the Service Worker and some caching features. Use a local server.

---

## 🎓 Who Is This For?

- Students preparing for **OPSC, OSSSC, OAS, OCS** exams
- Aspirants for **Railway (RRB), SSC CGL/CHSL, Banking** exams
- Anyone learning **Odia Grammar** or brushing up on **Lucent GK**
- Teachers and educators who want a free offline GK resource in Odia

---

## 🙏 Support the Project

If this app has helped your studies, consider supporting the developer:

[![Donate via Razorpay](https://img.shields.io/badge/💳%20Donate%20via%20Razorpay-FF6B6B?style=for-the-badge)](https://razorpay.me/@abhayabehera4628)

Your support helps keep the app free, ad-free, and actively maintained.

---

## 🔍 Keywords

`Odia GK` · `Odisha GK` · `Lucent GK Odia` · `Odia Grammar` · `ଓଡ଼ିଆ ବ୍ୟାକରଣ` · `OPSC preparation` · `OSSSC study material` · `Odia dictionary` · `GK mock test` · `offline GK app` · `PWA study app` · `competitive exam Odia` · `Lucent GK online` · `Odia MCQ test` · `GK by Abhaya`

---

## 📄 License

This project is free to use for educational purposes. Content sourced from Lucent Publications is used for educational/non-commercial study purposes only.

---

<div align="center">

Made with ❤️ by [Abhaya](https://github.com/abhayattcc) for Odia students everywhere.

**[⭐ Star this repo](https://github.com/abhayattcc/abhayagk)** if it helped you!

</div>
