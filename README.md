# 🔐 CompTIA Security+ SY0-701 Study App

<div align="center">

![Security+](https://img.shields.io/badge/CompTIA-Security%2B%20SY0--701-FF0000?style=for-the-badge&logo=comptia&logoColor=white)
![Questions](https://img.shields.io/badge/Questions-577-00D4FF?style=for-the-badge)
![No Framework](https://img.shields.io/badge/No%20Framework-Vanilla%20JS-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![Offline](https://img.shields.io/badge/Works-100%25%20Offline-22C55E?style=for-the-badge)

**A fully offline, browser-based study app for the CompTIA Security+ SY0-701 exam.**
Built with pure HTML, CSS & JavaScript — no install, no server, no internet required.

[🚀 Open the App](#getting-started) · [📚 Question Sources](#question-sources) · [✨ Features](#features)

</div>

---

## 📸 Overview

```
┌─────────────────────────────────────────────────────────┐
│  SY0-701 // Study App                                   │
│  Dashboard | Practice | Question Bank | Stats | Glossary│
├─────────────────────────────────────────────────────────┤
│                                                         │
│   ⏳ 26 Days Until Exam        📅 Today                │
│   ┌──────┐ ┌──────┐ ┌──────┐  Attempted:  12            │
│   │  26  │ │  04  │ │  32  │  Correct:     9            │
│   │ DAYS │ │  HRS │ │ MINS │  Accuracy:   75%           │
│   └──────┘ └──────┘ └──────┘                            │
│                                                         │
│   Domain Progress                                       │
│   ████████████████░░░░  General Security Concepts  80%  │ 
│   ██████████░░░░░░░░░░  Threats & Vulnerabilities  52%  │
│   ████████████████████  Security Architecture     100%  │
│                                                         │
└─────────────────────────────────────────────────────────┘
```

---

## ✨ Features

| Page | What it does |
|------|-------------|
| 🏠 **Dashboard** | Exam countdown to June 14 2026, today's accuracy, per-domain progress bars, weakest domain focus cards |
| ⚡ **Practice** | One question at a time, instant feedback, full explanation on wrong answers, session score tracker, filter by domain or session size |
| 📋 **Question Bank** | Full searchable table of all 577 questions, filter by domain or "got wrong before", add your own custom questions |
| 📊 **Stats** | 14-day accuracy chart, domain breakdown with pie chart, recent attempt history, reset progress |
| 📖 **Glossary** | 55+ key terms with A-Z filter and live search highlighting |

---

## 🚀 Getting Started

**Zero install. Just open a file.**

```bash
git clone https://github.com/Kavennesh/sec-_practice.git
cd sec-_practice
open index.html        # macOS
start index.html       # Windows
xdg-open index.html    # Linux
```

Or just double-click `index.html` in your file explorer.

> No Node.js. No npm. No build step. No internet after cloning.

---

## 📚 Question Sources

**577 total questions** extracted from two official study resources:

| Source | Book / File | Questions |
|--------|-------------|-----------|
| 📘 Mike Chapple & David Seidl | *CompTIA Security+ Study Guide, 9th Edition* | 333 |
| 🎓 Professor James Messer | *SY0-701 Practice Exams v1.8* — Exam A | 82 |
| 🎓 Professor James Messer | *SY0-701 Practice Exams v1.8* — Exam B | 80 |
| 🎓 Professor James Messer | *SY0-701 Practice Exams v1.8* — Exam C | 82 |
| **Total** | | **577** |

### Domain Breakdown

```
Domain 1 — General Security Concepts          ████████░░░░░░░  78 questions  (12%)
Domain 2 — Threats, Vulnerabilities & Mitig.  ████████████████ 151 questions  (26%)
Domain 3 — Security Architecture              ██████████░░░░░  98 questions  (17%)
Domain 4 — Security Operations                ██████████████░ 170 questions  (29%)
Domain 5 — Security Program Mgmt & Oversight  ████████░░░░░░░  80 questions  (14%)
```

Every question includes:
- ✅ Correct answer with full explanation
- ❌ Why each wrong answer is wrong
- 🏷️ SY0-701 exam objective mapping

---

## 🗂️ File Structure

```
sec-_practice/
├── index.html          # Dashboard
├── practice.html       # Practice questions
├── questions.html      # Question bank + add custom questions
├── stats.html          # Progress stats & charts
├── glossary.html       # Glossary with live search
├── style.css           # Shared dark theme styles
├── app.js              # Shared logic & localStorage helpers
└── data/
    ├── questions.js    # 577 questions (the whole bank)
    └── glossary.js     # 55+ Security+ key terms
```

---

## 💾 How Progress is Saved

All progress is saved automatically in your **browser's localStorage** — no account, no server, no cloud.

- Every answer attempt is recorded with timestamp
- Per-domain accuracy tracked over time
- 14-day daily accuracy history
- Custom questions you add persist between sessions
- Reset anytime from the Stats page

---

## 🎨 Design

- **Dark theme** — easy on the eyes during long study sessions
- **Color-coded domains** — each domain has its own accent color
- **Mobile friendly** — works on phone and tablet
- **Space Mono + DM Sans** — technical but readable typography

---

## 📅 Exam Target

> **June 14, 2026** — CompTIA Security+ SY0-701

The dashboard countdown updates in real time.

---

## 🤝 Contributing

Found a question error? Want to add more questions?

1. Fork the repo
2. Edit `data/questions.js` — follow the existing format:
```js
{
  id: 578,
  domain: "General Security Concepts",
  domainId: 1,
  question: `Your question text here?`,
  choices: { A: `Choice A`, B: `Choice B`, C: `Choice C`, D: `Choice D` },
  correct: "B",
  explanation: `Why B is correct, and why A, C, D are wrong.`
},
```
3. Open a Pull Request

Or use the **Add Custom Question** form inside the app itself — your custom questions save locally.

---

## 📜 License

Study materials are sourced from published exam prep books for personal educational use.
App code is MIT licensed.

---

<div align="center">

**Good luck on June 14th! 🎯**

*"The expert in anything was once a beginner."*

</div>
