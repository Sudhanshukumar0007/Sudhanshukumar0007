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

👋 About Me

I'm interested in the engineering side of AI — how models become reliable systems rather than just notebook experiments.

I work across backend engineering, distributed systems, and applied AI, with a particular interest in:

🤖 RAG systems and LLM applications

🧠 AI agents and tool-using systems

⚡ Async and real-time backends

🗄️ Databases, caching and distributed architectures

☁️ Cloud infrastructure and deployment

🧩 System design and scalable APIs

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

🚀 What I'm Building

Project

Description

Stack

LinkVault

Distributed URL shortener with analytics, rate limiting and background workers

FastAPI PostgreSQL Redis Celery

PulseRoom

Distributed real-time chat backend with multi-instance WebSocket communication

FastAPI WebSockets Redis PostgreSQL

Aaira

Modular AI desktop assistant with tools and persistent memory

FastAPI LangChain MongoDB ChromaDB

CognitiveSB

Open-source RAG study engine with multiple tutoring modes

LangGraph FAISS Flask Celery

📌 Featured Projects

⚡ PulseRoom

Distributed Real-Time Chat Backend

A backend project exploring the challenges of scaling real-time communication beyond a single application instance.

Designed distributed messaging using Redis Pub/Sub to fan out WebSocket events across application instances.

Implemented last_seen_message_id-based reconnect handling backed by durable PostgreSQL chat history.

Built ephemeral presence and typing indicators using Redis TTL keys.

Designed the system around horizontal scale-out of the application layer.

flowchart LR
    A[Client A] -->|WebSocket| I1[App Instance 1]
    B[Client B] -->|WebSocket| I2[App Instance 2]

    I1 <-->|Pub/Sub| R[(Redis)]
    I2 <-->|Pub/Sub| R

    I1 --> P[(PostgreSQL)]
    I2 --> P

Stack: FastAPI · AsyncIO · PostgreSQL · Redis · WebSockets · Docker Compose

🚀 Live Demo

🔗 LinkVault

Distributed URL Shortener & Analytics System

A backend project focused on API design, caching, asynchronous processing, authentication and abuse protection.

Designed and implemented 27+ automated integration tests using pytest, gated behind GitHub Actions CI.

Offloaded click analytics to Celery background workers behind a Redis cache-aside layer to keep the redirect path non-blocking.

Implemented atomic token revocation and sliding-window rate limiting using Redis sorted sets.

Added a fail-open fallback for Redis outages.

Structured the data layer using SQLAlchemy 2.0 async sessions and Alembic migrations.

flowchart LR
    U[User] --> API[FastAPI]

    API -->|Cache Aside| R[(Redis)]
    API --> DB[(PostgreSQL)]

    API -.->|Analytics Event| Q[[Celery Queue]]
    Q --> W[Celery Worker]
    W --> DB

Stack: FastAPI · PostgreSQL · Redis · Celery · SQLAlchemy · Alembic · Docker

🚀 Live API · 📂 Source

🤖 Aaira

Modular Agentic Desktop Assistant

An experimental AI assistant focused on tool use, memory and personalized interaction.

Built a multi-model pipeline using Llama 3.3, GPT-4o and Qwen3.

Integrated headless web browsing, shell execution, file I/O and UI control.

Added a confirmation gate before executing potentially sensitive actions.

Integrated InsightFace embeddings with ChromaDB and MongoDB for persistent personalized sessions.

Used WebSockets for real-time communication between the assistant and client.

Stack: FastAPI · LangChain · ChromaDB · MongoDB · WebSockets

📂 Source

🧠 CognitiveSB

Open-Source RAG Study Engine · GSSoC 2026

An AI-powered study platform built around retrieval-augmented generation and structured learning workflows.

Led development as GSSoC 2026 Project Admin, coordinating 10+ external contributors.

Reviewed and merged pull requests covering security fixes, asynchronous processing, FAISS session isolation and centralized validation.

Built an asynchronous LangGraph RAG pipeline supporting:

Socratic

Feynman

Simple Explanation

Exam Preparation

Processes PDFs and YouTube transcripts into structured notes and learning material.

Generates mind maps and SM-2 spaced-repetition flashcards.

Stack: LangChain · LangGraph · FAISS · Flask · Celery · Redis

📂 Source

🛠️ Tech Stack

Languages

<div align="center">

<img src="https://skillicons.dev/icons?i=python,cpp,java,ts,js,c,bash&perline=8" alt="Languages"/>

</div>

Backend & Databases

<div align="center">

<img src="https://skillicons.dev/icons?i=fastapi,flask,spring,postgres,mongodb,redis,sqlite&perline=8" alt="Backend and databases"/>

</div>

Cloud, DevOps & Infrastructure

<div align="center">

<img src="https://skillicons.dev/icons?i=docker,aws,github,githubactions,grafana,prometheus,git&perline=8" alt="Cloud and DevOps"/>

</div>

AI / ML

<div align="center">

LangChain · LangGraph · FAISS · ChromaDB · RAG · LLMs · Agents

</div>

🧠 Currently Exploring

<div align="center">

Distributed Systems · System Design · RAG Evaluation
AI Agents · LLM Serving · Backend Scalability

</div>

📊 GitHub Activity

<div align="center">

<img src="https://streak-stats.demolab.com?user=Sudhanshukumar0007&theme=tokyonight&hide_border=true" alt="GitHub streak"/>

</div>

🏆 Achievements & Certifications

☁️ AWS Certified Cloud Practitioner

🎓 Machine Learning Specialization — Coursera

🧩 330+ LeetCode problems solved in C++

🔥 57-day maximum LeetCode streak

🏅 1,627 LeetCode contest rating

🌍 GSSoC 2026 Project Admin

👨‍💻 Open-source contributor and project maintainer

Certificates

🎓 Machine Learning Specialization — Coursera

☁️ AWS Certified Cloud Practitioner

✍️ Writing

I write Backprop Diaries, documenting my AI/ML learning journey through experiments, concepts, failures and things I learn while building.

Read Backprop Diaries →

📫 Let's Connect

<div align="center">

<a href="https://github.com/Sudhanshukumar0007">
<img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white" alt="GitHub"/>
</a>

<a href="https://www.linkedin.com/in/sudhanshu-kumar-ai007/">
<img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"/>
</a>

<a href="mailto:sudhanshu.kumar.aidev007@gmail.com">
<img src="https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Email"/>
</a>

<a href="https://portfolio-nine-ecru-35.vercel.app/">
<img src="https://img.shields.io/badge/Portfolio-6C63FF?style=for-the-badge&logo=vercel&logoColor=white" alt="Portfolio"/>
</a>

<a href="https://leetcode.com/u/Sudhanshu_kumar_/">
<img src="https://img.shields.io/badge/LeetCode-FFA116?style=for-the-badge&logo=leetcode&logoColor=white" alt="LeetCode"/>
</a>

<a href="https://backpropdiaries.hashnode.dev">
<img src="https://img.shields.io/badge/Blog-2962FF?style=for-the-badge&logo=hashnode&logoColor=white" alt="Blog"/>
</a>

<br/><br/>

<img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=6,11,20&height=110&section=footer" width="100%" alt="footer"/>

</div>
