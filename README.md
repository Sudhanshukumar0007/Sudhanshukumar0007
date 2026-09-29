<!-- Header -->

<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=6,11,20&height=220&section=header&text=Sudhanshu%20Kumar&fontSize=54&fontColor=ffffff&animation=fadeIn&fontAlignY=38&desc=Backend%20%C2%B7%20Distributed%20Systems%20%C2%B7%20Applied%20AI&descAlignY=60&descSize=18" width="100%" alt="Sudhanshu Kumar"/>

<a href="https://github.com/Sudhanshukumar0007">
<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=22&pause=1200&color=00F7FF&center=true&vCenter=true&width=760&height=50&lines=B.Tech+CSE+(AI)+%40+KIET;Backend+%C2%B7+Distributed+Systems+%C2%B7+Applied+AI;Building+RAG+pipelines+and+AI+agents;Turning+experiments+into+real+systems" alt="Typing SVG"/>
</a>

<br/>

<img src="https://komarev.com/ghpvc/?username=Sudhanshukumar0007&label=Profile%20views&color=0e75b6&style=flat" alt="profile views"/>
<img src="https://img.shields.io/badge/CGPA-8.46-success?style=flat" alt="CGPA"/>
<img src="https://img.shields.io/badge/LeetCode-1627%20rating-FFA116?style=flat&logo=leetcode&logoColor=white" alt="LeetCode rating"/>
<img src="https://img.shields.io/badge/330%2B-LeetCode%20Problems-FFA116?style=flat&logo=leetcode&logoColor=white" alt="LeetCode problems"/>

</div>

---

## 👋 About Me

I'm interested in the engineering side of AI — **how models become reliable systems rather than just notebook experiments.**

I work across backend engineering, distributed systems, and applied AI, with a particular interest in:

* 🤖 RAG systems and LLM applications
* 🧠 AI agents and tool-using systems
* ⚡ Async and real-time backends
* 🗄️ Databases, caching and distributed architectures
* ☁️ Cloud infrastructure and deployment
* 🧩 System design and scalable APIs

```python
class Sudhanshu:
    role = "B.Tech CSE (AI) @ KIET"
    
    focus = [
        "Backend Engineering",
        "Distributed Systems",
        "Applied AI"
    ]

    currently = [
        "Building AI-powered systems",
        "Learning system design",
        "Contributing to open source"
    ]

    motto = "Make it work. Make it measurable. Make it ship."
```

---

## 🚀 What I'm Building

| Project         | Description                                                        | Stack                                       |
| --------------- | ------------------------------------------------------------------ | ------------------------------------------- |
| **PulseRoom**   | Real-time chat backend designed for multi-instance deployments     | `FastAPI` `WebSockets` `Redis` `PostgreSQL` |
| **LinkVault**   | URL shortener with analytics, rate limiting and background workers | `FastAPI` `PostgreSQL` `Redis` `Celery`     |
| **Aaira**       | Modular AI desktop assistant with tools and persistent memory      | `FastAPI` `LangChain` `MongoDB` `ChromaDB`  |
| **CognitiveSB** | Open-source RAG study engine with multiple tutoring modes          | `LangGraph` `FAISS` `Flask` `Celery`        |

---

## 📌 Featured Projects

### ⚡ PulseRoom

**Distributed real-time chat backend**

A backend designed to explore the problems that appear when a real-time application moves beyond a single server.

* WebSocket-based real-time communication
* Redis Pub/Sub for cross-instance event propagation
* PostgreSQL for durable message history
* Reconnection flow using the client's last-seen message ID
* Redis TTL keys for ephemeral presence and typing state

```mermaid
flowchart LR
    A[Client A] -->|WebSocket| I1[App Instance 1]
    B[Client B] -->|WebSocket| I2[App Instance 2]

    I1 <-->|Pub/Sub| R[(Redis)]
    I2 <-->|Pub/Sub| R

    I1 --> P[(PostgreSQL)]
    I2 --> P
```

**Stack:** FastAPI · AsyncIO · PostgreSQL · Redis · WebSockets · Docker

[📂 Source](https://github.com/Sudhanshukumar0007)

---

### 🔗 LinkVault

**URL shortener & analytics backend**

A backend project focused on API design, caching, asynchronous processing and abuse protection.

* Redis cache-aside strategy for frequently accessed data
* Celery workers for asynchronous analytics processing
* Sliding-window rate limiting using Redis sorted sets
* Token revocation
* PostgreSQL persistence
* SQLAlchemy 2.0 + Alembic migrations
* Automated testing with pytest and GitHub Actions

```mermaid
flowchart LR
    U[User] --> API[FastAPI]

    API -->|Cache Aside| R[(Redis)]
    API --> DB[(PostgreSQL)]

    API -.->|Analytics Event| Q[[Celery Queue]]
    Q --> W[Celery Worker]
    W --> DB
```

**Stack:** FastAPI · PostgreSQL · Redis · Celery · SQLAlchemy · Alembic · Docker

[📂 Source](https://github.com/Sudhanshukumar0007)

---

### 🤖 Aaira

**Modular agentic desktop assistant**

An experimental AI assistant exploring tool use, memory and multimodal interaction.

* Multi-model LLM pipeline
* Tool-based command execution
* Web browsing and file interaction
* Persistent conversation memory
* Face-recognition-based personalization
* ChromaDB + MongoDB for memory storage

**Stack:** FastAPI · LangChain · ChromaDB · MongoDB · WebSockets

[📂 Source](https://github.com/Sudhanshukumar0007)

---

### 🧠 CognitiveSB

**Open-source RAG study engine · GSSoC 2026**

An AI-powered study platform built around retrieval-augmented generation and structured learning workflows.

* LangGraph-based asynchronous RAG pipeline
* Four tutoring modes:

  * Socratic
  * Feynman
  * Simple Explanation
  * Exam Preparation
* PDF and YouTube transcript processing
* Structured notes and mind maps
* SM-2 spaced-repetition flashcards
* Celery + Redis for asynchronous workloads
* Open-source project administration and PR reviews

**Stack:** LangChain · LangGraph · FAISS · Flask · Celery · Redis

[📂 Source](https://github.com/Sudhanshukumar0007)

---

## 🛠️ Tech Stack

### Languages

<div align="center">

<img src="https://skillicons.dev/icons?i=python,cpp,java,ts,js,c,bash&perline=8" alt="Languages"/>

</div>

### Backend & Databases

<div align="center">

<img src="https://skillicons.dev/icons?i=fastapi,flask,spring,postgres,mongodb,redis,sqlite&perline=8" alt="Backend and databases"/>

</div>

### Cloud, DevOps & Infrastructure

<div align="center">

<img src="https://skillicons.dev/icons?i=docker,aws,github,githubactions,grafana,prometheus,git&perline=8" alt="Cloud and DevOps"/>

</div>

### AI / ML

<div align="center">

`LangChain` · `LangGraph` · `FAISS` · `ChromaDB` · `RAG` · `LLMs` · `Agents`

</div>

---

## 🧠 What I'm Learning

```text
Backend Engineering
├── API design
├── Async systems
├── Caching
├── Message queues
└── Distributed systems

Applied AI
├── RAG
├── Agent architectures
├── LLM evaluation
├── Embeddings
└── Model serving

System Design
├── Scalability
├── Reliability
├── Data consistency
├── Observability
└── Fault tolerance
```

---

## 📊 GitHub Activity

<div align="center">

<img height="180" src="https://github-readme-stats.vercel.app/api?username=Sudhanshukumar0007&show_icons=true&theme=tokyonight&hide_border=true&rank_icon=github" alt="GitHub stats"/>

<img height="180" src="https://github-readme-stats.vercel.app/api/top-langs/?username=Sudhanshukumar0007&layout=compact&theme=tokyonight&hide_border=true" alt="Top languages"/>

<br/>

<img src="https://streak-stats.demolab.com?user=Sudhanshukumar0007&theme=tokyonight&hide_border=true" alt="GitHub streak"/>

<br/>

<img src="https://github-readme-activity-graph.vercel.app/graph?username=Sudhanshukumar0007&theme=tokyo-night&hide_border=true&area=true" alt="GitHub activity graph" width="95%"/>

</div>

---

## 🏆 Achievements

* ☁️ **AWS Certified Cloud Practitioner**
* 🎓 **Machine Learning Specialization** — Coursera
* 🧩 **330+ LeetCode problems**
* 🔥 **57-day maximum LeetCode streak**
* 🏅 **1,627 LeetCode contest rating**
* 🌍 **GSSoC 2026 Project Admin**
* 👨‍💻 Open-source contributor and project maintainer

---

## ✍️ Writing

I document my AI/ML learning journey through **Backprop Diaries** — experiments, concepts, failures and things I learn while building.

**[Read Backprop Diaries →](https://backpropdiaries.hashnode.dev)**

---

## 📫 Connect

<div align="center">

<a href="https://github.com/Sudhanshukumar0007">
<img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white"/>
</a>

<a href="https://www.linkedin.com/in/YOUR-LINKEDIN">
<img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white"/>
</a>

<a href="mailto:sudhanshu.kumar.aidev007@gmail.com">
<img src="https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white"/>
</a>

<a href="https://YOUR-PORTFOLIO-URL">
<img src="https://img.shields.io/badge/Portfolio-6C63FF?style=for-the-badge&logo=vercel&logoColor=white"/>
</a>

<a href="https://backpropdiaries.hashnode.dev">
<img src="https://img.shields.io/badge/Blog-2962FF?style=for-the-badge&logo=hashnode&logoColor=white"/>
</a>

</div>

---

<div align="center">

### *Build → Measure → Learn → Ship*

<img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=6,11,20&height=110&section=footer" width="100%" alt="footer"/>

</div>
