<div align="center">

<!-- HERO BANNER -->
<br/>

```
███████╗██╗     ██╗███╗   ███╗██╗   ██╗    ██████╗ ██╗ ██████╗ ██╗████████╗ █████╗ ██╗
██╔════╝██║     ██║████╗ ████║██║   ██║    ██╔══██╗██║██╔════╝ ██║╚══██╔══╝██╔══██╗██║
█████╗  ██║     ██║██╔████╔██║██║   ██║    ██║  ██║██║██║  ███╗██║   ██║   ███████║██║
██╔══╝  ██║     ██║██║╚██╔╝██║██║   ██║    ██║  ██║██║██║   ██║██║   ██║   ██╔══██║██║
███████╗███████╗██║██║ ╚═╝ ██║╚██████╔╝    ██████╔╝██║╚██████╔╝██║   ██║   ██║  ██║███████╗
╚══════╝╚══════╝╚═╝╚═╝     ╚═╝ ╚═════╝     ╚═════╝ ╚═╝ ╚═════╝ ╚═╝   ╚═╝   ╚═╝  ╚═╝╚══════╝
```

<br/>

# 🎓 Elimu Digital

### Kenya's First AI-Powered CBC Learning Platform

**Built for Grade 7–9 students — to catch up, keep up, and excel.**

<br/>

[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg?style=for-the-badge)](LICENSE)
[![Node.js](https://img.shields.io/badge/Node.js-18+-339933?style=for-the-badge&logo=nodedotjs&logoColor=white)](https://nodejs.org)
[![React](https://img.shields.io/badge/React-18-61DAFB?style=for-the-badge&logo=react&logoColor=black)](https://react.dev)
[![PostgreSQL](https://img.shields.io/badge/PostgreSQL-14+-4169E1?style=for-the-badge&logo=postgresql&logoColor=white)](https://www.postgresql.org)
[![Powered by Claude](https://img.shields.io/badge/AI-Claude%20API-D4A843?style=for-the-badge)](https://anthropic.com)
[![PRs Welcome](https://img.shields.io/badge/PRs-Welcome-brightgreen?style=for-the-badge)](CONTRIBUTING.md)

<br/>

---

</div>

## 🌍 What is Elimu Digital?

> *"Elimu"* is the Swahili word for **education** — and that's exactly what this platform delivers.

Elimu Digital is a full-stack, AI-powered web platform built specifically for **Kenyan CBC (Competency-Based Curriculum)** students navigating the **Junior Secondary** transition (Grades 7–9). It meets students where they are, using intelligent tutoring, structured content, and gamification to make learning stick.

Whether a student is catching up on missed concepts, preparing for assessments, or aiming for the top of the class — Elimu Digital has them covered.

<br/>

---

## 🇰🇪 The CBC Structure

Kenya's reformed curriculum, as per **KICD guidelines**, is structured as follows:

| Stage | Duration | Level |
|---|---|---|
| 🟣 Pre-Primary | 2 years | PP1 – PP2 |
| 🟢 Primary | 6 years | Grade 1 – 6 |
| 🟡 **Junior Secondary** | **3 years** | **Grade 7 – 9** ← *Elimu Digital's primary focus* |
| 🔴 Senior Secondary | 3 years | Grade 10 – 12 |

> **Why Grade 7–9?** This is the most critical transition in the CBC pipeline — the move from primary to secondary school. New subjects, new teachers, new expectations. Elimu Digital bridges that gap.

<br/>

---

## ✨ Core Features

| Feature | Description |
|---|---|
| 📚 **Structured Notes** | KICD-aligned notes for every CBC subject and grade |
| 🤖 **AI Tutor** | Ask anything — get clear, grade-appropriate explanations powered by Claude |
| 📝 **Topic Quizzes** | Competency-based assessments with instant feedback |
| 📊 **Progress Tracking** | Visual dashboards per student, subject, and strand |
| 🏆 **Leaderboards & Streaks** | Gamified learning to keep students motivated |
| 👩‍🏫 **Teacher Dashboard** | Monitor class progress, identify struggling learners |
| 👨‍👩‍👧 **Parent Portal** | Stay informed with weekly reports and activity summaries |
| 🌐 **Offline-Ready** | Core content accessible with low/no internet (PWA support planned) |

<br/>

---

## 🧠 AI Tutor — Powered by Claude

The AI Tutor is the heart of Elimu Digital. Built on **Anthropic's Claude API**, it provides:

- **Socratic explanations** — doesn't just give answers, builds understanding
- **CBC-aligned language** — uses Kenya-specific curriculum terminology
- **Multi-subject support** — from Mathematics to Social Studies to Creative Arts
- **Grade-aware responses** — adapts complexity to the student's level (7, 8, or 9)
- **Swahili & English support** — students can ask in either language

<br/>

---

## 🛠️ Tech Stack

| Layer | Technology |
|---|---|
| **Frontend** | React 18 + Vite + TailwindCSS |
| **Backend** | Node.js + Express |
| **Database** | PostgreSQL 14+ + Prisma ORM |
| **Auth** | JWT + bcrypt |
| **AI Engine** | Anthropic Claude API |
| **Hosting** | Railway / Render (free tier) |
| **CDN** | Cloudflare |

<br/>

---

## 📁 Project Structure

```
elimu-digital/
├── frontend/                    # React 18 + Vite app
│   ├── src/
│   │   ├── components/          # Reusable UI components (cards, modals, nav)
│   │   ├── pages/               # Route pages: Home, Learn, Quiz, Dashboard
│   │   ├── hooks/               # Custom React hooks (useAuth, useProgress, useAI)
│   │   ├── lib/                 # API client, utilities, constants
│   │   └── styles/              # Global CSS + Tailwind config
│   └── public/                  # Static assets
│
├── backend/                     # Express REST API
│   ├── src/
│   │   ├── routes/              # API route definitions (auth, content, quiz, ai)
│   │   ├── controllers/         # Business logic handlers
│   │   ├── middleware/          # Auth, rate limiting, error handling
│   │   ├── models/              # Data models + types
│   │   └── services/            # AI service, email, analytics, leaderboard
│   └── prisma/
│       ├── schema.prisma        # Database schema
│       └── seed.ts              # Seed CBC curriculum data
│
├── docs/
│   ├── API.md                   # Full API reference
│   └── CURRICULUM.md            # CBC curriculum map (Grade 7–9 subjects & strands)
│
├── IMPLEMENTATION.md            # 👉 Detailed guide for Codex / AI code assistants
├── CONTRIBUTING.md              # How to contribute
└── README.md                    # You are here
```

<br/>

---

## 🚀 Quick Start

### Prerequisites

- **Node.js** 18+
- **PostgreSQL** 14+
- **npm** or **yarn**
- An **Anthropic API key** (get one at [console.anthropic.com](https://console.anthropic.com))

---

### 1. Clone the Repository

```bash
git clone https://github.com/your-org/elimu-digital.git
cd elimu-digital
```

---

### 2. Configure Environment Variables

```bash
# Copy example env files
cp backend/.env.example backend/.env
cp frontend/.env.example frontend/.env
```

Open `backend/.env` and fill in:

```env
DATABASE_URL="postgresql://user:password@localhost:5432/elimu_digital"
JWT_SECRET="your-secret-key-here"
ANTHROPIC_API_KEY="sk-ant-..."
PORT=4000
NODE_ENV=development
```

Open `frontend/.env` and fill in:

```env
VITE_API_URL=http://localhost:4000
```

---

### 3. Install Dependencies

```bash
# Backend
cd backend && npm install

# Frontend
cd ../frontend && npm install
```

---

### 4. Set Up the Database

```bash
cd backend

# Run migrations
npx prisma migrate dev --name init

# Seed with CBC curriculum content
npx prisma db seed
```

---

### 5. Start Development Servers

```bash
# Terminal 1 — Backend (http://localhost:4000)
cd backend && npm run dev

# Terminal 2 — Frontend (http://localhost:5173)
cd frontend && npm run dev
```

Open [http://localhost:5173](http://localhost:5173) — Elimu Digital is live. 🎉

<br/>

---

## 📚 CBC Subjects Covered (Grade 7–9)

| Subject | Grade 7 | Grade 8 | Grade 9 |
|---|:---:|:---:|:---:|
| Mathematics | ✅ | ✅ | ✅ |
| English | ✅ | ✅ | ✅ |
| Kiswahili | ✅ | ✅ | ✅ |
| Integrated Science | ✅ | ✅ | ✅ |
| Social Studies | ✅ | ✅ | ✅ |
| Religious Education (CRE/IRE/HRE) | ✅ | ✅ | ✅ |
| Creative Arts & Sports | ✅ | ✅ | ✅ |
| Agriculture & Nutrition | ✅ | ✅ | ✅ |
| Pre-Technical Studies | ✅ | ✅ | ✅ |
| Business Studies | ✅ | ✅ | ✅ |

> Content is mapped to KICD strands and sub-strands. See [`docs/CURRICULUM.md`](docs/CURRICULUM.md) for the full map.

<br/>

---

## 🚢 Deployment

### Free Tier Deployment (Recommended for MVP)

| Service | Used For | Free Tier |
|---|---|---|
| [Railway](https://railway.app) | Backend + PostgreSQL | 500 hrs/month |
| [Render](https://render.com) | Backend alternative | 750 hrs/month |
| [Vercel](https://vercel.com) | Frontend | Unlimited |
| [Cloudflare](https://cloudflare.com) | CDN + DNS | Free |

For the full step-by-step deployment guide, including environment setup, database migration on production, and CI/CD with GitHub Actions, see **[IMPLEMENTATION.md](IMPLEMENTATION.md)**.

<br/>

---

## 🤝 Contributing

Elimu Digital is an open educational project. Contributions from developers, educators, and curriculum experts are welcome.

```bash
# Fork → branch → PR
git checkout -b feature/your-feature-name
git commit -m "feat: add your feature"
git push origin feature/your-feature-name
```

Please read [CONTRIBUTING.md](CONTRIBUTING.md) before submitting a PR. Areas where help is especially needed:

- 📖 CBC content creation (subject notes, quiz questions)
- 🌐 Swahili localization
- ♿ Accessibility improvements
- 📱 Mobile UX / PWA support
- 🧪 Test coverage

<br/>

---

## 📄 License

**MIT © Elimu Digital 2025**

Free to use, modify, and distribute. If you build something with this, we'd love to hear about it — open an issue or reach out.

<br/>

---

<div align="center">

**Built with ❤️ for Kenyan students.**

*Catch up. Keep up. Excel.*

<br/>

[![Star this repo](https://img.shields.io/github/stars/your-org/elimu-digital?style=social)](https://github.com/your-org/elimu-digital)

</div>
