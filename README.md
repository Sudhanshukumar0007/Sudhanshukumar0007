<!-- Header banner -->
<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=6,11,20&height=220&section=header&text=Sudhanshu%20Kumar&fontSize=54&fontColor=ffffff&animation=fadeIn&fontAlignY=38&desc=Backend%20%C2%B7%20Distributed%20Systems%20%C2%B7%20Applied%20AI&descAlignY=60&descSize=18" width="100%" alt="header"/>

<!-- Typing animation -->
<a href="https://github.com/Sudhanshukumar0007">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=22&pause=1200&color=00F7FF&center=true&vCenter=true&width=760&height=50&lines=Second-year+CSE+(AI)+%40+KIET;Building+things+that+think;RAG+pipelines+%C2%B7+real-time+systems+%C2%B7+agents;Shipping+backends+that+survive+production" alt="Typing SVG" />
</a>

<br/>

<img src="https://komarev.com/ghpvc/?username=Sudhanshukumar0007&label=Profile%20views&color=0e75b6&style=flat" alt="profile views"/>
<img src="https://img.shields.io/badge/CGPA-8.46-success?style=flat&logo=googlescholar&logoColor=white" alt="cgpa"/>
<img src="https://img.shields.io/badge/LeetCode-1627%20rating-FFA116?style=flat&logo=leetcode&logoColor=white" alt="leetcode"/>
<img src="https://img.shields.io/badge/Open%20to-Remote%20AI%2FML%20Internships-8A2BE2?style=flat" alt="open to work"/>

</div>

---

## 👋 About me

I'm obsessed with the gap between **"a model that works in a notebook"** and **"a system that actually ships."**
Most of my work lives in that gap: RAG pipelines, real-time systems, and full-stack apps with AI baked in.

```python
class Sudhanshu:
    role     = "B.Tech CSE (AI) @ KIET, 2024-2028"
    focus    = ["Backend", "Distributed Systems", "LLM apps"]
    currently = ["Leading GSSoC 2026 project", "Writing Backprop Diaries", "Building in public"]
    certs    = ["AWS Cloud Practitioner", "ML Specialization (Coursera)"]

    def motto(self):
        return "Make it work, make it measurable, make it ship."
```

---

## 🚀 What I'm building right now

| Project | What it does | Stack |
|---|---|---|
| **[PulseRoom](https://github.com/Sudhanshukumar0007)** | Real-time chat backend that scales horizontally across instances | `FastAPI` `WebSockets` `Redis Pub/Sub` |
| **[LinkVault](https://github.com/Sudhanshukumar0007)** | URL shortener with non-blocking analytics, rate limiting and RBAC | `FastAPI` `PostgreSQL` `Redis` `Celery` `Docker` |
| **[Aaira](https://github.com/Sudhanshukumar0007)** | Agentic desktop assistant with face recognition and cross-session memory | `LangChain` `ChromaDB` `MongoDB` |
| **[CognitiveSB](https://github.com/Sudhanshukumar0007)** | Open-source RAG study engine with four tutoring modes | `LangGraph` `FAISS` `Flask` `Celery` |

---

## 📌 Featured projects

> 👇 Click any project to expand the details and architecture.

<details>
<summary><b>⚡ PulseRoom</b> — Distributed real-time chat backend</summary>
<br/>

- Fans out WebSocket events over **Redis Pub/Sub**, so multiple app instances can serve one chat room.
- **No message loss on reconnect:** clients send `last_seen_message_id` and catch up from durable PostgreSQL history.
- **Presence and typing indicators** use ephemeral Redis TTL keys, so there is no persistent state to clean up.

```mermaid
flowchart LR
    A[Client A] -->|WebSocket| I1[App instance 1]
    B[Client B] -->|WebSocket| I2[App instance 2]
    I1 <-->|publish / subscribe| R[(Redis Pub/Sub)]
    I2 <-->|publish / subscribe| R
    I1 --> P[(PostgreSQL history)]
    I2 --> P
```

**Stack:** FastAPI · AsyncIO · PostgreSQL · Redis · WebSockets · Docker Compose
[🔗 Live demo](https://github.com/Sudhanshukumar0007) · [📂 Source](https://github.com/Sudhanshukumar0007)

</details>

<details>
<summary><b>🔗 LinkVault</b> — URL shortener & analytics system</summary>
<br/>

- **27+ integration tests** (pytest) gated behind a GitHub Actions CI pipeline.
- **Fast redirects:** click analytics are offloaded to Celery workers behind a Redis cache-aside layer.
- **Abuse protection:** atomic token revocation and sliding-window rate limiting on Redis sorted sets, with a fail-open fallback if the cache goes down.
- **Safe schema changes** via SQLAlchemy 2.0 async sessions and Alembic migrations.

```mermaid
flowchart LR
    U[User] --> API[FastAPI]
    API -->|cache-aside| RC[(Redis)]
    API --> DB[(PostgreSQL)]
    API -.->|enqueue click event| Q[[Celery queue]]
    Q --> W[Celery workers]
    W --> DB
```

**Stack:** FastAPI · PostgreSQL · Redis · Celery · SQLAlchemy · Alembic · Docker
[🔗 Live API](https://github.com/Sudhanshukumar0007) · [📂 Source](https://github.com/Sudhanshukumar0007)

</details>

<details>
<summary><b>🤖 Aaira</b> — Modular agentic desktop assistant</summary>
<br/>

- Multi-model pipeline (**Llama 3.3, GPT-4o, Qwen3**) that parses and executes commands.
- Tools: headless web browsing, shell execution, file I/O and UI control, all behind a **secure confirmation gate**.
- **Face recognition + memory:** InsightFace embeddings stored in ChromaDB and MongoDB for personalized, persistent sessions.

**Stack:** FastAPI · LangChain · ChromaDB · MongoDB · WebSocket
[📂 Source](https://github.com/Sudhanshukumar0007)

</details>

<details>
<summary><b>🧠 CognitiveSB</b> — Open-source RAG study engine (GSSoC 2026 · Project Admin)</summary>
<br/>

- Coordinating **10+ external contributors** and reviewing and merging PRs, including a path traversal security fix, Celery/Redis async integration, FAISS session isolation and centralized validation.
- Async **LangGraph** RAG pipeline with four tutoring modes: *Socratic, Feynman, Simple, Exam Prep*.
- Turns PDFs and YouTube transcripts into structured notes, mind maps and **SM-2 spaced-repetition flashcards**.

**Stack:** LangChain · LangGraph · FAISS · Flask · Celery · Redis
[📂 Source](https://github.com/Sudhanshukumar0007)

</details>

---

## 🛠️ Tech stack

<div align="center">

**Languages**<br/>
<img src="https://skillicons.dev/icons?i=python,cpp,java,ts,js,c,bash&perline=8" alt="languages"/>

**Backend & Data**<br/>
<img src="https://skillicons.dev/icons?i=fastapi,flask,spring,postgres,mongodb,redis,sqlite&perline=8" alt="backend"/>

**DevOps & Cloud**<br/>
<img src="https://skillicons.dev/icons?i=docker,aws,github,githubactions,grafana,prometheus,git&perline=8" alt="devops"/>

**AI / ML** — LangChain · LangGraph · FAISS · ChromaDB · RAG · LLMs

</div>

---

## 📊 GitHub stats

<div align="center">

<img height="180" src="https://github-readme-stats.vercel.app/api?username=Sudhanshukumar0007&show_icons=true&theme=tokyonight&hide_border=true&rank_icon=github" alt="stats"/>
<img height="180" src="https://github-readme-stats.vercel.app/api/top-langs/?username=Sudhanshukumar0007&layout=compact&theme=tokyonight&hide_border=true" alt="top languages"/>

<img src="https://streak-stats.demolab.com?user=Sudhanshukumar0007&theme=tokyonight&hide_border=true" alt="streak"/>

<img src="https://github-readme-activity-graph.vercel.app/graph?username=Sudhanshukumar0007&theme=tokyo-night&hide_border=true&area=true" alt="activity graph" width="95%"/>

</div>

<!-- Optional: contribution snake (needs the snk GitHub Action, see notes) -->
<!--
<div align="center">
  <img src="https://raw.githubusercontent.com/Sudhanshukumar0007/Sudhanshukumar0007/output/github-snake-dark.svg" alt="snake"/>
</div>
-->

---

## 🏆 Achievements & certifications

- ☁️ **AWS Certified Cloud Practitioner**
- 🎓 **Machine Learning Specialization** — Coursera (Andrew Ng)
- 🧩 **330+ LeetCode problems** in C++ · 57-day max streak · contest rating **1,627** (top 20.87% globally)
- 🌍 **GSSoC 2026 Project Admin** — leading an open-source AI project end to end

---

## ✍️ Writing

I write **[Backprop Diaries](https://backpropdiaries.hashnode.dev)**, documenting my AI/ML learning journey in public.

---

## 📫 Let's connect

<div align="center">

<a href="https://github.com/Sudhanshukumar0007"><img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white"/></a>
<a href="https://www.linkedin.com/in/YOUR-LINKEDIN"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white"/></a>
<a href="mailto:sudhanshu.kumar.aidev007@gmail.com"><img src="https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white"/></a>
<a href="https://YOUR-PORTFOLIO-URL"><img src="https://img.shields.io/badge/Portfolio-6C63FF?style=for-the-badge&logo=vercel&logoColor=white"/></a>
<a href="https://backpropdiaries.hashnode.dev"><img src="https://img.shields.io/badge/Blog-2962FF?style=for-the-badge&logo=hashnode&logoColor=white"/></a>

<br/><br/>

<img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=6,11,20&height=110&section=footer" width="100%" alt="footer"/>

</div>
