<div align="center">

[![Typing SVG](https://readme-typing-svg.demolab.com?font=Fira+Code&weight=700&size=26&pause=1200&color=58A6FF&center=true&vCenter=true&width=850&lines=Hey%2C+I'm+Ayush+Ranjan+%F0%9F%91%8B;I+build+AI+that+admits+when+it+doesn't+know.;Agents+%C2%B7+RAG+%C2%B7+RL+%C2%B7+Vision+%C2%B7+Uncertainty;LLM+post-training+%C2%B7+published+cryptography+research)](https://git.io/typing-svg)

[![LinkedIn](https://img.shields.io/badge/LinkedIn-%230077B5.svg?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/ayush-ranjan-1b0a47300)
[![Gmail](https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:ayushranjan1271@gmail.com)
[![Codeforces](https://img.shields.io/badge/Codeforces-1F8ACB?style=for-the-badge&logo=codeforces&logoColor=white)](https://codeforces.com/profile/Ayush_Ranjan12)
[![Paper](https://img.shields.io/badge/%F0%9F%93%84_Published_Paper-00C853?style=for-the-badge)](https://iads.site/a-new-approach-for-image-security-enhancement-using-ternary-logic-linear-feedback-shift-register-for-cryptographic-applications/)
[![Portfolio](https://img.shields.io/badge/%F0%9F%8C%90_Portfolio-FF5722?style=for-the-badge)](https://ayush-1271.github.io/)

[![Profile Views](https://hits.sh/github.com/Ayush-1271.svg?style=flat-square&label=Profile%20Views&color=58A6FF)](https://hits.sh/github.com/Ayush-1271/)

</div>

---

### 🧠 Agents & LLM Systems

| | |
|---|---|
| **[🧠 NoteMind](https://github.com/Ayush-1271/NoteMind)** — `Multi-Agent AI · Graph Memory`<br>LangChain, AutoGen and CrewAI agents each live in an isolated context window, so token costs explode as swarms grow. NoteMind gives a 4-agent swarm (PM → Frontend → Backend → QA, **Gemini 2.5**) a **persistent semantic knowledge graph** instead. Agents write atomic Markdown notes, indexed in **ChromaDB + MongoDB**, and retrieve only the relevant slice. Live graph visualization in **React Flow** over **FastAPI WebSockets**. | **[📄 RAG PDF Chat](https://github.com/Ayush-1271/rag-pdf-chat)** — `Full-Stack RAG` · [**Live demo**](https://rag-pdf-chat-seven.vercel.app/)<br>Ask a PDF questions and get answers grounded in the document with **page-level citations**. A **7-agent pipeline** (extract → analyze → preprocess → optimize → synthesize → validate → assemble), **FAISS** per-session indexes, **SSE token streaming**, and **automatic failover** across OpenRouter, Groq, Gemini, Hugging Face and OpenAI. React + TypeScript + FastAPI + LangChain. |
| **[🔍 MangaLens](https://github.com/Ayush-1271/MangaLens)** — `Multimodal · Chrome Extension`<br>Google Translate skips text inside images, and the story in manga lives in speech bubbles. MangaLens uses **Gemini Vision** to detect text in panels, translate it into 18 languages, and **redraw it in place**. It keeps a **translation memory** so character names stay consistent across pages. The README lists its limits honestly, too. | **[📋 AI Resume Analyzer](https://github.com/Ayush-1271/AI_Resume_Analyzer)** — `NLP`<br>Scores a resume against a job description with a **3-signal hybrid** (TF-IDF + `all-MiniLM-L6-v2` embeddings + skill overlap), finds missing skills against a 10k+ skill vocabulary, ranks jobs, and runs on **OpenVINO** so no CUDA is needed. Streamlit UI included. |

```mermaid
flowchart LR
    U[User prompt] --> PM[Project Manager]
    PM --> FE[Frontend Engineer]
    FE --> BE[Backend Engineer]
    BE --> QA[QA Tester]
    PM -.writes notes.-> G[(Knowledge Graph)]
    FE -.writes notes.-> G
    BE -.writes notes.-> G
    QA -.writes notes.-> G
    G -.semantic retrieval.-> FE
    G -.semantic retrieval.-> BE
    G -.semantic retrieval.-> QA
```

---

### 🎯 Reasoning Under Uncertainty & Reinforcement Learning

| | |
|---|---|
| **[📈 MarketLens](https://github.com/Ayush-1271/MarketLens)** — `Probabilistic ML · RAPID framework`<br>**Not** a trading bot. A regime-aware system that outputs **P10 / P50 / P90 bands** instead of point predictions, classifies volatility regimes with a **CNN + Transformer** model, **rejects assets with unreliable data**, and returns `NaN` rather than a fabricated metric. Stress-tested on the COVID-19 crash. Streamlit dashboard included. | **[🕹️ PPO Agents + Live Demo](https://github.com/Ayush-1271/rl-demo-web)** — `Reinforcement Learning`<br>**[CartPole](https://github.com/Ayush-1271/cartpole-ppo-rl)**: perfect **500/500**. **[LunarLander](https://github.com/Ayush-1271/lunarlander-ppo-rl)**: mean **~251** (solved is 200; a random agent scores about -178). The trained policies are exported to **pure NumPy weights** and verified for 100% action agreement with Stable-Baselines3, so the **[Flask web demo](https://github.com/Ayush-1271/rl-demo-web)** runs live episodes without PyTorch. |

> 🔐 **[Published research →](https://iads.site/a-new-approach-for-image-security-enhancement-using-ternary-logic-linear-feedback-shift-register-for-cryptographic-applications/)** Ternary Logic LFSR for cryptographic S-box design in image security, evaluated with NPCR, UACI and entropy analysis.

---

### 👁️ Vision & Classical ML (built from the math up)

| Project | What it does | Result |
|---|---|---|
| **[🫁 Cancer Detection CNN](https://github.com/Ayush-1271/cancer-detection-cnn)** | 5-block deep CNN classifying lung histopathology (adenocarcinoma, squamous cell, normal) on 15,000 images | **96.98%** accuracy · **0.9963** AUC |
| **[🙂 Face Recognition CNN](https://github.com/Ayush-1271/face-recognition-cnn)** | 15-class face recognition on LFW with a custom deep CNN | **86.23%** val accuracy |
| **[🎬 Movie Recommender](https://github.com/Ayush-1271/Movie-Recommendation-System)** | Collaborative filtering with **Truncated SVD implemented from scratch** (pandas, NumPy, SciPy; no recsys libraries) on MovieLens, a matrix that is 98.3% empty | Top-5 picks per user |
| **[🎓 TeachAI](https://github.com/Ayush-1271/TeachAI)** | Anti-proxy attendance using **face recognition + GPS validation** | Built for real classrooms |

---

### ⭐ Passion Project: Novel Vault

> *Not for a resume, not for a class. I built it because I wanted it to exist.*

**A modular web-novel aggregation, caching, download and document-generation platform.** Search several novel sites at once, cache chapters on disk, download in the background, survive crashes, and export clean **PDF / EPUB / TXT** books.

| | |
|---|---|
| **🧩 Plugin architecture** | `BaseSource` for sites, `OutputFormat` for exports. Plugins self-register via decorators and are auto-discovered, so new sites or formats never touch the core workflow. |
| **🌐 4 source adapters** | FanMTL, NovelFire (Requests + BeautifulSoup) · TomatoMTL, WTR-Lab (Selenium automation). |
| **🔎 Concurrent cross-source search** | Dispatched to every adapter in parallel, normalized, exact-title filtered. |
| **⚙️ Resumable pipeline** | `pending → running → completed / failed / cancelled`. Cancel, retry, resume. Cached chapters are never fetched twice. |
| **🔐 Browser-driven login** | Sign in via a real Chrome window; cookies are stored, validated and expiry-checked before each job. |
| **🛡️ Reliability** | HTTP retry/backoff, block detection, fresh-session Selenium retries, orphaned-job recovery after restarts, graceful browser cleanup. |
| **🧪 Tested** | Unit, integration and contract tests across adapters, outputs, lifecycle, APIs and search. |

```mermaid
flowchart LR
    A[Pick novel, range, batch, format] --> B[Download record]
    B --> C[Auth + format pre-flight]
    C --> D[Background worker]
    D --> E{Cached?}
    E -- yes --> G[Reuse from disk]
    E -- no --> F[Scrape + cache]
    F --> G
    G --> H[PDF / EPUB / TXT batches]
    H --> I[Progress + status]
```

`Python` `FastAPI` `SQLAlchemy 2.0` `SQLite` `Selenium` `BeautifulSoup4` `Jinja2` `Vanilla JS` `fpdf2` `EbookLib` `pytest`

🔒 **Private repository**

---

### 🔭 More Explorations

| Repo | What I was curious about |
|---|---|
| **[⚗️ ChemicalEquipmentVisualizer](https://github.com/Ayush-1271/ChemicalEquipmentVisualizer)** | Can one **Django REST API** be the single source of truth for a **React web app and a PyQt5 desktop app** at once? |
| **[🩺 Diabetes Progression API](https://github.com/Ayush-1271/diabetes-risk-predictor-docker)** | A Flask ML API shipped in **Docker**, using only the 5 inputs a person could actually know from a checkup. |
| **[💬 Social Media Sentiment Analysis](https://github.com/Ayush-1271/Social-Media-Sentiment-Analysis)** | How far do classic NLP + ML classifiers go on messy social text? |
| **[📚 Bin2Book Novel Scraper](https://github.com/Ayush-1271/Bin2Book-Novel-Scraper)** | A multi-threaded scraper with a GUI that turns web novels into structured PDFs. |
| **[🌊 waipy (fork)](https://github.com/Ayush-1271/waipy)** | Wavelet analysis: continuous wavelet transform, significance tests, cross-wavelet analysis. |

---

### 🛠️ Stack

**Languages**
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![Java](https://img.shields.io/badge/Java-ED8B00?style=flat-square&logo=openjdk&logoColor=white)
![C++](https://img.shields.io/badge/C++-00599C?style=flat-square&logo=c%2B%2B&logoColor=white)
![C](https://img.shields.io/badge/C-A8B9CC?style=flat-square&logo=c&logoColor=black)
![SQL](https://img.shields.io/badge/SQL-4479A1?style=flat-square&logo=mysql&logoColor=white)

**AI / ML**
![PyTorch](https://img.shields.io/badge/Stable--Baselines3-EE4C2C?style=flat-square&logo=pytorch&logoColor=white)
![TensorFlow](https://img.shields.io/badge/TensorFlow-FF6F00?style=flat-square&logo=tensorflow&logoColor=white)
![LangChain](https://img.shields.io/badge/LangChain-1C3C3C?style=flat-square&logo=langchain&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=flat-square&logo=scikit-learn&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=flat-square&logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=flat-square&logo=numpy&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=flat-square&logo=jupyter&logoColor=white)
![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=flat-square&logo=streamlit&logoColor=white)

**Backend, Data & Automation**
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![Django](https://img.shields.io/badge/Django-092E20?style=flat-square&logo=django&logoColor=white)
![Flask](https://img.shields.io/badge/Flask-000000?style=flat-square&logo=flask&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=flat-square&logo=mongodb&logoColor=white)
![SQLite](https://img.shields.io/badge/SQLite-003B57?style=flat-square&logo=sqlite&logoColor=white)
![Selenium](https://img.shields.io/badge/Selenium-43B02A?style=flat-square&logo=selenium&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)

**Frontend & Tools**
![React](https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=react&logoColor=black)
![Tailwind](https://img.shields.io/badge/Tailwind-06B6D4?style=flat-square&logo=tailwindcss&logoColor=white)
![Firebase](https://img.shields.io/badge/Firebase-FFCA28?style=flat-square&logo=firebase&logoColor=black)
![AWS](https://img.shields.io/badge/AWS-232F3E?style=flat-square&logo=amazon-aws&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)
![Chrome Extension](https://img.shields.io/badge/Chrome_Extension-4285F4?style=flat-square&logo=google-chrome&logoColor=white)

---

### 🎮 Side Quests

- ⚔️ Competitive programming on [Codeforces](https://codeforces.com/profile/Ayush_Ranjan12) · 300+ problems solved on LeetCode
- 📖 Web novels and manga are why **Novel Vault** and **MangaLens** exist
- 🔐 Cryptography, from a published paper on ternary-logic LFSRs

---

### 📊 Stats

<div align="center">

[![GitHub Streak](https://streak-stats.demolab.com/?user=Ayush-1271&theme=github-dark-blue&hide_border=true&date_format=j%20M%5B%20Y%5D)](https://git.io/streak-stats)

</div>

---

<div align="center">

*Open to ML/NLP internships, research collaborations, and interesting hard problems.*

**[📬 ayushranjan1271@gmail.com](mailto:ayushranjan1271@gmail.com)**

</div>
