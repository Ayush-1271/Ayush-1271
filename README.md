<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0D1117,50:1F6FEB,100:58A6FF&height=210&section=header&text=Ayush%20Ranjan&fontSize=58&fontColor=FFFFFF&fontAlignY=38&desc=AI%20%2F%20ML%20Engineer%20%C2%B7%20Researcher%20%C2%B7%20Systems%20Tinkerer&descSize=18&descAlignY=60" width="100%" alt="Ayush Ranjan banner"/>

[![Typing SVG](https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=20&pause=1400&color=58A6FF&center=true&vCenter=true&width=820&lines=I+build+AI+that+admits+when+it+doesn't+know.;Multi-agent+memory+%C2%B7+RAG+%C2%B7+RL+%C2%B7+Vision+%C2%B7+Uncertainty;Ex-LLM+post-training+intern+%C2%B7+published+cryptography+researcher;Curious+first.+Then+I+build+it%2C+break+it%2C+and+measure+it.)](https://git.io/typing-svg)

<br/>

[![LinkedIn](https://img.shields.io/badge/LinkedIn-%230077B5.svg?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/ayush-ranjan-1b0a47300)
[![Portfolio](https://img.shields.io/badge/Portfolio-FF5722?style=for-the-badge&logo=githubpages&logoColor=white)](https://ayush-1271.github.io/)
[![Paper](https://img.shields.io/badge/Published_Paper-00C853?style=for-the-badge&logo=readthedocs&logoColor=white)](https://iads.site/a-new-approach-for-image-security-enhancement-using-ternary-logic-linear-feedback-shift-register-for-cryptographic-applications/)
[![Codeforces](https://img.shields.io/badge/Codeforces-1F8ACB?style=for-the-badge&logo=codeforces&logoColor=white)](https://codeforces.com/profile/Ayush_Ranjan12)
[![Gmail](https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:ayushranjan1271@gmail.com)

[![Profile Views](https://hits.sh/github.com/Ayush-1271.svg?style=flat-square&label=Profile%20Views&color=58A6FF)](https://hits.sh/github.com/Ayush-1271/)

</div>

<br/>

<table align="center">
<tr>
<td align="center"><b>Integrated M.Tech</b><br/>Computational & Data Science<br/>VIT Bhopal</td>
<td align="center"><b>LLM Post-Training</b><br/>Intern @ <a href="https://ethara.ai">Ethara.ai</a><br/>(completed)</td>
<td align="center"><b>Published</b><br/>Ternary Logic LFSR<br/>for image cryptography</td>
<td align="center"><b>Certified</b><br/>Google IT Support<br/>Professional</td>
</tr>
</table>

---

## Scoreboard

<table align="center">
<tr>
<td align="center"><h3>500 / 500</h3>CartPole (PPO)<br/>perfect score</td>
<td align="center"><h3>~251</h3>LunarLander (PPO)<br/>solved at 200</td>
<td align="center"><h3>96.98%</h3>Lung histopathology CNN<br/>0.9963 AUC</td>
<td align="center"><h3>7 agents</h3>RAG pipeline<br/>5-provider LLM failover</td>
</tr>
</table>

---

## Flagship Projects

<table>
<tr>
<td width="50%" valign="top">

### [NoteMind](https://github.com/Ayush-1271/NoteMind)
**Graph memory for multi-agent AI**

Every agent framework gives each agent an isolated context window, so token cost explodes as swarms grow. NoteMind replaces that with a **persistent semantic knowledge graph**: agents write atomic Markdown notes, retrieve only the relevant slice, and you watch the graph grow live.

`Gemini 2.5` `FastAPI` `WebSockets` `ChromaDB` `MongoDB` `React Flow`

</td>
<td width="50%" valign="top">

### [RAG PDF Chat](https://github.com/Ayush-1271/rag-pdf-chat) · [Live demo](https://rag-pdf-chat-seven.vercel.app/)
**Chat with a PDF, with page-level citations**

A **7-agent answer pipeline** (extract → analyze → preprocess → optimize → synthesize → validate → assemble), a **FAISS index per session**, **SSE token streaming**, and **automatic failover** across OpenRouter, Groq, Gemini, Hugging Face and OpenAI.

`React` `TypeScript` `FastAPI` `LangChain` `FAISS`

</td>
</tr>
<tr>
<td width="50%" valign="top">

### [MarketLens](https://github.com/Ayush-1271/MarketLens)
**Market analysis that admits when it doesn't know**

Not a trading bot. A **CNN + Transformer** model outputs **P10 / P50 / P90 bands**, classifies volatility regimes, **rejects unreliable assets**, and returns `NaN` instead of a fabricated metric. Stress-tested on the COVID-19 crash.

`CNN + Transformer` `Probabilistic forecasting` `Streamlit`

</td>
<td width="50%" valign="top">

### Novel Vault · *private repository*
**My passion project. Built because I wanted it to exist.**

A modular web-novel **aggregation, caching, download and document-generation platform**: plugin-based source adapters and export formats, concurrent cross-source search, a resumable background pipeline, browser-driven login, and PDF / EPUB / TXT output.

`FastAPI` `SQLAlchemy` `Selenium` `BeautifulSoup` `fpdf2` `EbookLib` `pytest`

</td>
</tr>
</table>

<details>
<summary><b>Under the hood: how NoteMind agents share memory</b></summary>

<br/>

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

</details>

<details>
<summary><b>Under the hood: how Novel Vault downloads a book</b></summary>

<br/>

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

| Capability | Detail |
|---|---|
| Plugin architecture | `BaseSource` for sites and `OutputFormat` for exports; plugins self-register and are auto-discovered |
| Source adapters | FanMTL, NovelFire (Requests + BeautifulSoup) · TomatoMTL, WTR-Lab (Selenium) |
| Search | Concurrent across all adapters, normalized, exact-title filtered |
| Download lifecycle | pending → running → completed / failed / cancelled, with retry, resume and cancel |
| Reliability | HTTP backoff, block detection, fresh-session Selenium retries, orphaned-job recovery, disk-backed chapter cache |

</details>

---

## How I Work

| | |
|---|---|
| **Honest evaluation** | MarketLens returns `NaN` instead of a made-up score. MangaLens documents exactly what it can't do. I'd rather show a limit than hide it. |
| **Memory beats brute force** | NoteMind, RAG PDF Chat and Novel Vault all avoid redoing work: retrieve the relevant slice, cache what's already done. |
| **Ship it so people can touch it** | PPO agents run live in a browser demo, a RAG app is deployed, and models are exported to lightweight NumPy so demos stay fast on free tiers. |

---

## The Lab

<details open>
<summary><b>More AI & LLM projects</b></summary>

<br/>

| Project | What it does |
|---|---|
| **[MangaLens](https://github.com/Ayush-1271/MangaLens)** | Chrome extension. **Gemini Vision** finds text inside manga panels, translates it into 18 languages, and redraws it in place, with a **translation memory** to keep character names consistent. |
| **[AI Resume Analyzer](https://github.com/Ayush-1271/AI_Resume_Analyzer)** | **3-signal hybrid** match score (TF-IDF + MiniLM embeddings + skill overlap), skill-gap analysis against a 10k+ vocabulary, job ranking, and OpenVINO inference (no CUDA needed). |
| **[Social Media Sentiment Analysis](https://github.com/Ayush-1271/Social-Media-Sentiment-Analysis)** | NLP + classical ML classifiers on messy social text. |

</details>

<details>
<summary><b>Reinforcement learning</b></summary>

<br/>

| Project | Result |
|---|---|
| **[CartPole PPO](https://github.com/Ayush-1271/cartpole-ppo-rl)** | Perfect **500/500** every evaluation episode (random agent: ~27) |
| **[LunarLander PPO](https://github.com/Ayush-1271/lunarlander-ppo-rl)** | Mean **~251**, solved threshold 200 (random agent: ~-178), ~1.11M timesteps |
| **[RL Demo Web](https://github.com/Ayush-1271/rl-demo-web)** | Flask app that runs live episodes of both agents. Policies are exported to **pure NumPy** and verified for **100% action agreement** with Stable-Baselines3. |

</details>

<details>
<summary><b>Vision & classical ML</b></summary>

<br/>

| Project | Result |
|---|---|
| **[Cancer Detection CNN](https://github.com/Ayush-1271/cancer-detection-cnn)** | **96.98%** accuracy · **0.9963** AUC on 15,000 lung histopathology images |
| **[Face Recognition CNN](https://github.com/Ayush-1271/face-recognition-cnn)** | **86.23%** validation accuracy, 15 classes on LFW |
| **[Movie Recommender](https://github.com/Ayush-1271/Movie-Recommendation-System)** | Collaborative filtering with **Truncated SVD from scratch** on a 98.3%-empty matrix |
| **[TeachAI](https://github.com/Ayush-1271/TeachAI)** | Anti-proxy attendance: **face recognition + GPS validation** |
| **[Diabetes Progression API](https://github.com/Ayush-1271/diabetes-risk-predictor-docker)** | Flask ML API deployed with **Docker**, using only inputs a person can actually know |

</details>

<details>
<summary><b>Full-stack & tooling experiments</b></summary>

<br/>

| Project | What it does |
|---|---|
| **[ChemicalEquipmentVisualizer](https://github.com/Ayush-1271/ChemicalEquipmentVisualizer)** | One **Django REST API** powering both a **React web app** and a **PyQt5 desktop app** |
| **[Bin2Book Novel Scraper](https://github.com/Ayush-1271/Bin2Book-Novel-Scraper)** | Multi-threaded scraper with a GUI that turns web novels into structured PDFs |
| **[waipy (fork)](https://github.com/Ayush-1271/waipy)** | Wavelet analysis: CWT, significance tests, cross-wavelet analysis |

</details>

> **Research:** [Ternary Logic LFSR for cryptographic S-box design](https://iads.site/a-new-approach-for-image-security-enhancement-using-ternary-logic-linear-feedback-shift-register-for-cryptographic-applications/), evaluated with NPCR, UACI and entropy analysis.

---

## Toolbox

<div align="center">

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![Java](https://img.shields.io/badge/Java-ED8B00?style=flat-square&logo=openjdk&logoColor=white)
![C++](https://img.shields.io/badge/C++-00599C?style=flat-square&logo=c%2B%2B&logoColor=white)
![C](https://img.shields.io/badge/C-A8B9CC?style=flat-square&logo=c&logoColor=black)
![SQL](https://img.shields.io/badge/SQL-4479A1?style=flat-square&logo=mysql&logoColor=white)
<br/>
![TensorFlow](https://img.shields.io/badge/TensorFlow-FF6F00?style=flat-square&logo=tensorflow&logoColor=white)
![Stable-Baselines3](https://img.shields.io/badge/Stable--Baselines3-EE4C2C?style=flat-square&logo=pytorch&logoColor=white)
![LangChain](https://img.shields.io/badge/LangChain-1C3C3C?style=flat-square&logo=langchain&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=flat-square&logo=scikit-learn&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=flat-square&logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=flat-square&logo=numpy&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=flat-square&logo=jupyter&logoColor=white)
![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=flat-square&logo=streamlit&logoColor=white)
<br/>
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![Django](https://img.shields.io/badge/Django-092E20?style=flat-square&logo=django&logoColor=white)
![Flask](https://img.shields.io/badge/Flask-000000?style=flat-square&logo=flask&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=flat-square&logo=mongodb&logoColor=white)
![SQLite](https://img.shields.io/badge/SQLite-003B57?style=flat-square&logo=sqlite&logoColor=white)
![Selenium](https://img.shields.io/badge/Selenium-43B02A?style=flat-square&logo=selenium&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
<br/>
![React](https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=react&logoColor=black)
![Tailwind](https://img.shields.io/badge/Tailwind-06B6D4?style=flat-square&logo=tailwindcss&logoColor=white)
![Firebase](https://img.shields.io/badge/Firebase-FFCA28?style=flat-square&logo=firebase&logoColor=black)
![AWS](https://img.shields.io/badge/AWS-232F3E?style=flat-square&logo=amazon-aws&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)

</div>

---

## Off the Clock

- Competitive programming: [Codeforces](https://codeforces.com/profile/Ayush_Ranjan12) · 300+ problems solved on LeetCode
- Web novels and manga are the reason **Novel Vault** and **MangaLens** exist
- Cryptography, from a published paper on ternary-logic LFSRs

<br/>

<div align="center">

[![GitHub Streak](https://streak-stats.demolab.com/?user=Ayush-1271&theme=github-dark-blue&hide_border=true&date_format=j%20M%5B%20Y%5D)](https://git.io/streak-stats)

<br/>

*Open to ML/NLP internships, research collaborations, and interesting hard problems.*

**[ayushranjan1271@gmail.com](mailto:ayushranjan1271@gmail.com)**

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0D1117,50:1F6FEB,100:58A6FF&height=110&section=footer" width="100%" alt=""/>

</div>
