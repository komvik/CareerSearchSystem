# CareerSearchSystem
Modular AI job search pipeline with FastAPI, Ollama LLM integration, Google Drive storage, and n8n automation workflows.




AI-powered job search automation system that helps streamline the entire job application process using artificial intelligence, automation workflows, and cloud storage.

## 🚀 Overview

CareerSearchSystem is a modular system designed to transform job searching into a structured, automated, and repeatable workflow.

It integrates AI analysis, document management, and automation tools to assist with:

- Job collection and tracking  
- Job description analysis  
- CV and cover letter generation  
- Application management  
- Automated workflows and notifications  

---

## 🧠 Core Concept

Instead of manually applying to jobs, the system builds an automated pipeline:

1. Collect job postings  
2. Analyze job requirements using AI (Ollama / LLMs)  
3. Match with user profile  
4. Generate optimized CV and cover letters  
5. Store and manage documents via Google Drive  
6. Automate workflows using n8n  
7. Track application status and improvements  

---

## 🏗 Architecture

- **Frontend:** HTML / React (dashboard UI)
- **Backend:** FastAPI / Node.js
- **AI Engine:** Ollama (local LLM models)
- **Automation:** n8n workflows
- **Storage:** Google Drive API
- **Database:** SQLite / PostgreSQL
- **Deployment:** Docker (planned)

---

## 📁 Project Structure

CareerSearchSystem/
│
├── backend/
├── frontend/
├── n8n/
├── docker/
├── docs/
├── .env.example
└── README.md


---

## ⚙️ Features (MVP)

- Google Drive integration for document storage  
- AI-based job description analysis  
- CV and cover letter generation  
- Basic job tracking system  
- Automated workflow triggers (n8n)  

---

## 🔧 Tech Stack

- Python (FastAPI)  
- JavaScript (React / Node.js)  
- Ollama (LLMs)  
- n8n (automation)  
- Google Drive API  
- Docker (deployment)

---

## 📌 Status

This project is currently in active development (MVP stage).

---

## 📜 License

MIT License
CareerSearchSystem/
│
├── backend/                          # 🧠 Core API (FastAPI)
│   ├── app/
│   │   ├── api/                     # REST endpoints
│   │   ├── services/                # business logic
│   │   │   ├── ai_service.py       # Ollama integration
│   │   │   ├── drive_service.py     # Google Drive logic
│   │   │   ├── job_service.py      # job parsing / analysis
│   │   │   └── cv_service.py       # CV / letter generation
│   │   │
│   │   ├── core/                   # config, settings
│   │   ├── models/                 # DB models
│   │   ├── schemas/                # Pydantic schemas
│   │   ├── db/                     # database setup
│   │   └── main.py                 # entry point
│   │
│   ├── tests/
│   ├── requirements.txt
│   ├── Dockerfile
│   └── .env.example
│
│
├── frontend/                        # 🌐 UI (React or simple HTML)
│   ├── src/
│   ├── public/
│   ├── pages/
│   ├── components/
│   ├── services/                   # API calls to backend
│   ├── index.html
│   └── package.json
│
│
├── n8n/                             # ⚙️ Automation workflows
│   ├── workflows/
│   │   ├── job_scraper.json
│   │   ├── daily_analysis.json
│   │   └── notifications.json
│   └── README.md
│
│
├── docker/                          # 🐳 Infrastructure
│   ├── docker-compose.yml
│   ├── backend.Dockerfile
│   ├── frontend.Dockerfile
│   └── n8n.Dockerfile (optional)
│
│
├── database/                        # 🗄️ Local DB (dev only)
│   ├── migrations/
│   └── seed/
│
│
├── integrations/                    # 🔌 External APIs layer
│   ├── google_drive/
│   │   ├── auth.py
│   │   ├── client.py
│   │   └── files.py
│   │
│   ├── ollama/
│   │   ├── client.py
│   │   └── prompts.py
│   │
│   └── n8n/
│       └── webhook_handlers.py
│
│
├── docs/                            # 📚 Documentation
│   ├── architecture.md
│   ├── api.md
│   └── workflows.md
│
│
├── scripts/                         # 🛠️ utility scripts
│   ├── setup.sh
│   ├── run_backend.sh
│   └── deploy.sh
│
│
├── storage/                         # 📂 local files (ignored in git)
│   ├── cv/
│   ├── letters/
│   ├── jobs/
│   └── outputs/
│
│
├── .env.example                     # 🔐 environment template
├── .gitignore
├── README.md
└── LICENSE