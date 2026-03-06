<div align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:0D1B2A,100:5BC0BE&height=180&section=header&text=Uddesh%20Singh&fontColor=F2A541&fontSize=80&animation=fadeIn&fontAlignY=40" width="100%"/>
  
  <a href="https://git.io/typing-svg">
    <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=24&pause=1000&color=F2A541&center=true&vCenter=true&width=600&lines=MS+CS+%40+UT+Dallas;Full-Stack+%26+Cloud+Engineer;AI+%26+Machine+Learning+Enthusiast" alt="Typing SVG" />
  </a>
  <br/>
  <img src="https://komarev.com/ghpvc/?username=uddeshsingh&color=5BC0BE&style=flat-square&label=PROFILE+VIEWS" alt="Visitor Counter" />
</div>

<div align="center">
  <a href="https://linkedin.com/in/uddesh-singh">
    <img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"/>
  </a>
  <a href="mailto:uddeshsingh@gmail.com">
    <img src="https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white" alt="Email"/>
  </a>
  <a href="https://github.com/uddeshsingh">
    <img src="https://img.shields.io/badge/Github-181717?style=for-the-badge&logo=github&logoColor=white" alt="Github"/>
  </a>
  <a href="https://leetcode.com/uddeshsingh">
    <img src="https://img.shields.io/badge/LeetCode-FFA116?style=for-the-badge&logo=leetcode&logoColor=black" alt="LeetCode"/>
  </a>
</div>

---

### About Me

I am a Master's student in **Computer Science** at the **University of Texas at Dallas** (GPA 4.0), actively seeking New Graduate and Entry-Level Software Engineering roles. I am passionate about building scalable distributed systems, network architectures, and AI-driven applications.

- 💼 **Latest Role:** Software Development Intern at **Paycom** (working on .NET/React & OCR engines).
- 🏢 **Previous Experience:** Senior Associate of Development at **American Express**, where I designed, developed and scaled internal tools using Python, Golang and GCP.
- 🏆 **Achievements:** Paycom Code-a-thon Winner (2025) & Gupta Fellow at UT Dallas.
- ⚡ **Interests:** High-concurrency systems, Cloud Architecture (AWS/GCP), and Generative AI (RAG pipelines).

---

### GitHub Achievements

<div align="center">
  <a href="https://github.com/ryo-ma/github-profile-trophy">
    <img src="https://github-profile-trophy.vercel.app/?username=uddeshsingh&theme=dracula&no-bg=true&column=7&margin-w=15" alt="trophy" />
  </a>
</div>

---

### Tech Stack & Tools

| **Category**          | **Technologies**                                                                                                                  |
| :-------------------- | :-------------------------------------------------------------------------------------------------------------------------------- |
| **Languages**         | <img src="https://skillicons.dev/icons?i=py,go,java,cs,cpp,js,ts&theme=dark" align="middle" />                                    |
| **Backend & Cloud**   | <img src="https://skillicons.dev/icons?i=django,dotnet,nodejs,aws,gcp,docker,kubernetes,kafka,linux&theme=dark" align="middle" /> |
| **Databases & Cache** | <img src="https://skillicons.dev/icons?i=postgres,mysql,redis&theme=dark" align="middle" />                                       |
| **Frontend & Tools**  | <img src="https://skillicons.dev/icons?i=react,git,githubactions&theme=dark" align="middle" />                                    |

---

### Featured Projects

| Project                               | Tech Stack                               | Description                                                                                                                 |
| :------------------------------------ | :--------------------------------------- | :-------------------------------------------------------------------------------------------------------------------------- |
| **Distributed Real-Time Watch Party** | `Golang` `Redis` `WebSockets` `React`    | Architected a **distributed system** handling 10k+ concurrent users via **sharding** and **event-driven** message delivery. |
| **Network Path Visualizer**           | `Python` `React` `Graph Algorithms`      | Built a highly interactive tool for visualizing complex network routing, pathing, and architectural topologies.             |
| **AI Financial Analyst (SIA)**        | `LangChain` `FAISS` `Gemini`             | Built a financial advisor using a Retrieval-Augmented Generation (RAG) system for sub-second vector search retrieval.       |
| **Cloud-Native AI Video Generator**   | `Kubernetes` `FastAPI` `Celery` `FFmpeg` | Designed a containerized video pipeline, auto-scaling worker nodes to reduce processing time by 90%.                        |

#### 🏗️ WatchParty Architecture

```mermaid
graph TD
    %% Custom Styles
    classDef frontend fill:#0D1B2A,stroke:#5BC0BE,stroke-width:2px,color:#FFF
    classDef routing fill:#F2A541,stroke:#0D1B2A,stroke-width:2px,color:#000
    classDef compute fill:#1B263B,stroke:#5BC0BE,stroke-width:2px,color:#FFF
    classDef state fill:#415A77,stroke:#F2A541,stroke-width:2px,color:#FFF
    classDef db fill:#336791,stroke:#FFF,stroke-width:2px,color:#FFF
    classDef storage fill:#8C3061,stroke:#FFF,stroke-width:1px,color:#FFF

    subgraph "🌐 Client Tier"
        UI["💻 React SPA (Video & Chat)"]:::frontend
    end

    subgraph "🚦 Network & Edge"
        CDN["📦 CloudFront/CDN (Static Assets)"]:::routing
        LB["⚖️ Cloud Load Balancer (WSS/GRPC)"]:::routing
    end

    subgraph "⚙️ Go Microservices"
        WS["🟢 WebSocket Handler (Sharded)"]:::compute
        API["🔵 REST API (Auth & Rooms)"]:::compute
        WORKER["🟣 Async Worker (Video Processing)"]:::compute
    end

    subgraph "⚡ Real-Time Layer"
        PUBSUB["📢 Redis Pub/Sub (Event Bus)"]:::state
        CACHE[("🗄️ Redis (Session & Lock)")]:::state
    end

    subgraph "💾 Data & Storage"
        DB[("🐘 PostgreSQL (Users & History)")]:::db
        S3[("☁️ S3/GCS (Video Content)")]:::storage
    end

    %% Flow Connections
    UI --"HTTPS (Fetch Assets)"--> CDN
    UI <== "WSS (Persistent)" ==> LB
    LB ==> WS
    LB ==> API

    WS <-->|Broadcasting| PUBSUB
    WS <-->|Sync State| CACHE

    API -->|Auth/CRUD| DB
    WORKER --"Scan/Process"--> S3
    WORKER --"Save Metadata"--> DB
    API --"Enqueue Task"--> CACHE
```

---

### Daily Analytics

<div align="center">
<img src="https://raw.githubusercontent.com/uddeshsingh/uddeshsingh/main/github-metrics.svg" width="48%">
<img src="https://leetcard.jacoblin.cool/uddeshsingh?theme=dark&font=Fira%20Code&ext=activity" width="48%" alt="LeetCode Stats" />
</div>

---

### Contributions

<div align="center">
<picture>
<source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/uddeshsingh/uddeshsingh/output/github-contribution-snake-dark.svg">
<source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/uddeshsingh/uddeshsingh/output/github-contribution-snake.svg">
<img alt="github contribution grid snake animation" src="https://raw.githubusercontent.com/uddeshsingh/uddeshsingh/output/github-contribution-snake.svg">
</picture>
</div>
