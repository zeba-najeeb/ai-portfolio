# ⚡ Zeba Najeeb | AI Solutions Architect & Developer

<p align="left">
  <b>Generative AI Solutions Architecture • Enterprise RAG Systems • Agentic Workflows • FastAPI Backend Automation</b>
</p>

<p align="left">
  📍 <b>Location:</b> Sharjah / Dubai, United Arab Emirates<br>
  💼 <b>Current Role:</b> AI Solutions Architect & Developer at Unique Computer Systems (UCS)<br>
  🚀 <b>Live Flagship AI App:</b> <a href="https://zeba-ai-job-hunter.streamlit.app"><b>Autonomous AI Job Hunter & RAG Career Co-Pilot</b></a><br>
  📫 <b>Contact:</b> <a href="mailto:zebarishab@gmail.com">zebarishab@gmail.com</a> |
  <a href="https://www.linkedin.com/in/zeba-najeeb">LinkedIn Profile</a> |
  <a href="https://github.com/zeba-najeeb">GitHub Profile</a>
</p>

<p align="left">
  <a href="https://zeba-ai-job-hunter.streamlit.app"><img src="https://static.streamlit.io/badges/streamlit_badge_black_white.svg" alt="Live App on Streamlit"></a>
  <a href="https://fastapi.tiangolo.com/"><img src="https://img.shields.io/badge/FastAPI-Async%20REST-009688?logo=fastapi&logoColor=white" alt="FastAPI"></a>
  <a href="https://ai.google.dev/"><img src="https://img.shields.io/badge/LLMs-Google%20Gemini-8E75C2?logo=google&logoColor=white" alt="Google Gemini"></a>
  <a href="https://www.langchain.com/"><img src="https://img.shields.io/badge/Orchestration-LangChain%20%7C%20LangGraph-1C3C3C?logo=langchain&logoColor=white" alt="LangChain and LangGraph"></a>
  <a href="https://www.trychroma.com/"><img src="https://img.shields.io/badge/Vector%20DB-ChromaDB-blue" alt="ChromaDB"></a>
  <a href="https://www.python.org/"><img src="https://img.shields.io/badge/Python-3.12%2B-3776AB?logo=python&logoColor=white" alt="Python"></a>
  <a href="https://www.docker.com/"><img src="https://img.shields.io/badge/Containers-Docker-2496ED?logo=docker&logoColor=white" alt="Docker"></a>
</p>

---

## 👨‍💻 Executive Summary

Results-driven **AI Solutions Architect & Developer** specializing in designing and deploying scalable **Generative AI applications, production-oriented Retrieval-Augmented Generation (RAG) systems, and high-throughput asynchronous APIs**.

Experienced in taking AI products from architectural design to enterprise deployment, including developing the AI core for **Qualif AI**, a recruitment intelligence platform designed to automate candidate screening and evaluation.

Skilled in LLM prompt engineering, structured output validation, vector search optimization, high-concurrency backend development with FastAPI, and multi-agent workflows.

---

## 🌟 Commercial Case Study: Enterprise Production

### 🏆 Qualif AI — Recruitment & Candidate Intelligence Platform

- **Company:** Unique Computer Systems (UCS), Dubai, UAE
- **Role:** AI Solutions Architect & Developer
- **Responsibilities:** AI architecture, LLM integration, evaluation logic, and automation pipelines
- **Status:** Launched and deployed in commercial SaaS production

#### System Architecture

```text
┌─────────────────────────────────────────────────────────────────────┐
│                  QUALIF AI SYSTEM ARCHITECTURE                      │
├─────────────────────────────────────────────────────────────────────┤
│                                                                     │
│  Candidate Ingestion       Evaluation Core        Delivery & Audit  │
│                                                                     │
│  [IMAP Email Monitor] ──► [PDF Resume Parsing] ──► [Candidate      │
│          │                         │                Reports]        │
│          ▼                         ▼                    │           │
│  [FastAPI Async API] ──► [LLM-Based Evaluation]        ▼           │
│          │                         │              [Email Alerts]    │
│          ▼                         ▼                    │           │
│  [APScheduler Worker]     [Scoring & Gap Analysis]      ▼           │
│                                                 [SQLite Audit Trail]│
└─────────────────────────────────────────────────────────────────────┘
```

#### Key Deliverables & Business Impact

- **Candidate Screening Automation:** Developed automated workflows to parse, standardize, and evaluate candidate resumes against job requirements. The platform was reported to reduce manual screening effort by approximately **70%**.
- **Automated Ingestion:** Implemented a background processing workflow using IMAP/SMTP and APScheduler to monitor and process incoming applications, with a reported processing volume of **50+ applications daily**.
- **Structured Candidate Evaluation:** Designed LLM-based evaluation pipelines with structured output validation to generate candidate match scores, skills comparisons, and gap analyses.
- **Asynchronous Backend:** Developed FastAPI endpoints and offloaded blocking operations using `asyncio` executor patterns to support concurrent PDF processing and I/O-intensive tasks.
- **Auditability:** Integrated SQLite-based logging to maintain records of processed applications and evaluation results.

---

## 🚀 Flagship Open-Source AI Platform (Live Cloud Demo)

### 🎯 Autonomous AI Job Hunter & RAG Career Co-Pilot

- **Live Cloud Application:** **[zeba-ai-job-hunter.streamlit.app](https://zeba-ai-job-hunter.streamlit.app)**
- **Source Code Repository:** **[github.com/zeba-najeeb/autonomous-ai-job-hunter](https://github.com/zeba-najeeb/autonomous-ai-job-hunter)**
- **Core Stack:** Python 3.12, Google Gemini 2.5 API & Embeddings (`3072-dim`), ChromaDB, PyMuPDF, SQLite, Pydantic v2, Streamlit

#### Architectural Highlights
- **Multi-Tenant Ephemeral Vector Store (`ChromaDB`):** Parses any candidate PDF resume into overlapping semantic chunks (`chunk_size=800`, `overlap=150`) with strict `candidate_id` tenant isolation and an automated **7-day sliding inactivity TTL** to maintain near-zero cloud disk usage.
- **Stateful Portal Queue & Smart Discovery Adapter:** Recommends regional job portals for any target city/country, persists progression (`PENDING` → `IN_PROGRESS` → `COMPLETED`) in SQLite, and routes discovery across Google Search Index Grounding and Open APIs.
- **2-Stage Quality Gate (`<= 30 Days` + Global Deduplication):** Normalizes relative timestamps to filter out expired listings older than 30 days and computes deterministic SHA-256 job fingerprints (`company + normalized_title`) to prevent cross-portal duplicates.
- **RAG Semantic Scoring & On-Demand Co-Pilot (`>= 70%` Gate):** Evaluates active openings against retrieved CV chunks (`0–100%` score + skill gap analysis) and unlocks a 4-tab Career Co-Pilot (Zero-Hallucination ATS CV Bullets, Tailored Cover Letter, Skill-Gap Roadmap, and CV-Grounded Interview Q&A).

---

## 🛠️ Open-Source AI Systems & Engineering Projects

| Project | Technology Stack | Key Highlights | Links |
|---|---|---|---|
| **Autonomous AI Job Hunter & RAG Co-Pilot** *(Flagship)* | Gemini 2.5, ChromaDB, PyMuPDF, SQLite, Pydantic v2, Streamlit | Multi-tenant RAG job matcher (`0–100%`), stateful portal queue, `<=30d` freshness gate, and 4-tab AI Career Co-Pilot. | [🚀 Live App](https://zeba-ai-job-hunter.streamlit.app) • [📦 GitHub](https://github.com/zeba-najeeb/autonomous-ai-job-hunter) |
| **Enterprise RAG Knowledge Assistant** | LangChain, ChromaDB, Llama 3, FastAPI | RAG pipeline with document chunking, conversational history, retrieval, and hallucination-reduction techniques. | [Explore Repository](https://github.com/zeba-najeeb/ai-business-assistant) |
| **Agentic Decision Workflows** | LangGraph, Python, Tool Calling, StateGraph | Stateful agent workflows with conditional branching, human-in-the-loop review, and iterative retrieval. | [Explore Repository](https://github.com/zeba-najeeb/Langgraph1) |
| **AI Python Tutor & Interactive Chatbot** | Python, LLMs, Prompt Engineering, Gradio/UI | Context-aware coding mentor designed to explain concepts, debug code, and guide learners interactively. | [Explore Repository](https://github.com/zeba-najeeb/python-tutor-chatbot) |
| **Dubai Real Estate Valuation Engine** | Python, Scikit-learn, Pandas, XGBoost | Machine learning project for estimating property prices across Dubai communities. | [Explore Repository](https://github.com/zeba-najeeb/Dubai_Apartment_Price-Prediction) |

---

## 🧰 Technical Competencies

### 🧠 Generative AI & Orchestration

- **LLMs & APIs:** Google Gemini, Llama, OpenAI APIs, Hugging Face Transformers
- **Frameworks:** LangChain, LangGraph, Rasa
- **RAG Architecture:** Document ingestion, text chunking, embeddings, vector search, retrieval strategies, conversational memory, and prompt guardrails
- **Agentic AI:** Tool calling, stateful workflows, conditional routing, multi-agent coordination, and human-in-the-loop review
- **LLM Reliability:** Structured outputs, validation, prompt engineering, and hallucination mitigation

### ⚡ Backend, Concurrency & Document Processing

- **Frameworks:** FastAPI, Django, Flask, REST API design
- **Python:** Async/await, Pydantic, asyncio, modular application architecture
- **Document Processing:** PyMuPDF (`fitz`), BeautifulSoup4, ReportLab, Jinja2
- **Background Processing:** APScheduler, IMAP/SMTP integration, scheduled tasks, and worker offloading
- **Data Processing:** NumPy, Pandas

### 🗄️ Databases, DevOps & Tools

- **Databases:** ChromaDB, SQLite, MySQL, MongoDB
- **DevOps:** Docker, Git, GitHub
- **Development Tools:** Postman, Antigravity CLI, Cursor, Linux, Windows PowerShell

---

## 📜 Education & Certifications

- **M.Tech in Communication Engineering & Signal Processing** — MES College of Engineering  
  CGPA: 7.65/10
- **B.Tech in Electronics & Communication Engineering** — LBS Institute of Technology for Women (LBSITW)
- **IBM / Coursera:** *Build RAG Applications: Get Started*, *Develop Generative AI Applications*, *Python for Data Science & AI*
- **LangChain Unleashed:** *A Guide to Using Open Source LLM Models*

---

## 🤝 Let's Connect

I am open to opportunities and professional discussions related to **AI Solutions Architecture, Generative AI Engineering, RAG Development, and AI Automation**, particularly across the UAE and with global remote teams.

- 🌐 **LinkedIn:** [linkedin.com/in/zeba-najeeb](https://www.linkedin.com/in/zeba-najeeb)
- 📧 **Email:** [zebarishab@gmail.com](mailto:zebarishab@gmail.com)
- 📍 **Location:** Sharjah / Dubai, United Arab Emirates

---

<p align="center">
  <i>Building practical AI solutions that connect intelligent models with real-world business needs.</i>
</p>
