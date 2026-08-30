# Angel Mishra

**Java Backend Developer | Full-Stack Software Engineer**  
B.Tech in Electronics & Communication Engineering — **Banasthali Vidyapith**  
*Machine Learning & Computer Vision Research Exposure (NIT Kurukshetra Internship & Final Year Project)*

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Angel_Mishra-0A66C2?style=flat&logo=linkedin)](https://www.linkedin.com/in/angel-mishra-992474345/)
[![GitHub](https://img.shields.io/badge/GitHub-123angmish-181717?style=flat&logo=github)](https://github.com/123angmish)

---

## 👨‍💻 Professional Summary

I am a software engineer focused on building robust, secure backend systems in **Java & Spring Boot** and dynamic full-stack applications with **React.js**. I emphasize writing clean, testable code, enforcing strong authentication & authorization boundaries, designing relational database schemas, and applying efficient Data Structures & Algorithms to solve practical engineering problems.

- 🔭 **Current Focus**: Building secure RESTful APIs, Spring Security authentication architectures, and learning database concurrency & transaction management.
- 🎯 **Target Roles**: Java Backend Developer, Full-Stack Developer, Software Development Engineer (SDE).
- 💡 **Core CS**: Data Structures & Algorithms, Object-Oriented Programming (OOP), Database Management Systems (DBMS), Operating Systems, Computer Networks.

---

## 🛠️ Technical Stack

| Area | Technologies |
| :--- | :--- |
| **Backend & APIs** | Java 21, Spring Boot (3.x), Spring Security 6, Spring Data JPA, Hibernate, RESTful APIs, JWT, BCrypt, Jakarta Validation |
| **Frontend** | React.js, Redux Toolkit, JavaScript (ES6+), HTML5, CSS3, Tailwind CSS, Vite |
| **Databases & ORM** | PostgreSQL, MySQL, H2 Database, Hibernate ORM, Flyway Database Migrations |
| **Tools & Environments** | Git, GitHub, Maven, Docker, Postman, Linux / Bash, MVC Architecture |
| **ML & Computer Vision** | Python 3.10+, FastAPI, OpenCV, MobileNetV2 / TensorFlow, Librosa, Scikit-Learn |

---

## 🌟 Featured Placement Projects

### 1. [CampusShare](https://github.com/123angmish/campus-share-project-) — Peer-to-Peer Campus Marketplace *(Flagship Project)*
*Full-stack campus utility sharing platform built with Java 21, Spring Boot 3.5, React 19, and PostgreSQL.*
- **Concurrency & Locking**: Implemented pessimistic database row-locking (`SELECT FOR UPDATE`) and optimistic versioning to prevent double-booking collisions during concurrent rental requests.
- **Security & Authorization**: Stateless JWT authentication paired with rotating HttpOnly refresh tokens; backend-enforced ownership checks on all listing mutations.
- **Payment Architecture**: Razorpay order workflow with server-side HMAC-SHA256 signature verification and an idempotent durable webhook inbox for reliable payment settlement.
- **Stack**: Java 21, Spring Boot 3.5, React 19, PostgreSQL 16, Flyway, Spring Security, Docker.

---

### 2. [HireVia](https://github.com/123angmish/hire-via-job-portal) — Recruitment & Applicant Tracking System
*Full-stack job portal and talent acquisition platform with role-based access control and live ATS workflow.*
- **Security Hardening**: Stateless JWT authentication with externalized secret configuration, BCrypt salt hashing, in-memory rate limiting against brute-force attacks, and server-side IDOR protection across jobs and applicant data.
- **Secure Messaging & ATS**: Candidate-employer communication channel with JWT-derived identity verification and an ATS pipeline (`APPLIED` ➔ `SHORTLISTED` ➔ `INTERVIEW` ➔ `HIRED`/`REJECTED`).
- **Stack**: Java 21, Spring Boot 3.5, React 18, Vite, Redux Toolkit, Tailwind CSS, Spring Security 6.

---

### 3. [AI Virality Predictor](https://github.com/123angmish/ai-virality-predictor) — Video Intelligence & Platform Optimizer *(NIT Kurukshetra Research Internship Project)*
*Multimodal video analytics engine and regression benchmark evaluating video pacing across YouTube Shorts, TikTok, and Instagram Reels.*
- **Feature Extraction**: Extracted optical motion flow (0–3s hook intensity) via OpenCV and acoustic RMS energy peaks via Librosa.
- **Machine Learning Benchmark**: Baseline regression comparison on a controlled synthetic multimodal benchmark ($N=10,000$) where Linear Regression proved optimal ($R^2 = 0.8824$, $\text{RMSE} = 4.5194$) due to the underlying linear target structure.
- **Project Evolution**: Originated as a Flask research prototype during my NIT Kurukshetra internship, later independently expanded into a FastAPI + Next.js 14 platform with automated platform blueprints.
- **Stack**: Python, FastAPI, Next.js 14, OpenCV, Librosa, Scikit-Learn, Tailwind CSS.

---

### 4. [FloodGuard AI](https://github.com/123angmish/floodguard-ai) — Real-Time Flood Hazard & Risk Monitoring *(Final Year Computer Vision Project)*
*AI and Computer Vision prototype developed as a Final Year Project in B.Tech ECE (Banasthali Vidyapith) for flood-scene analysis, estimated surface motion/flow analysis, and community risk alerting.*
- **Computer Vision Pipeline**: Combines a MobileNetV2-based CNN for frame-level flood scene classification with Lucas-Kanade optical flow for relative surface motion tracking and estimated flow analysis.
- **Verified Architecture**: Saved model contains a MobileNetV2-based frozen backbone (~2.26M non-trainable parameters) with a custom dense binary classification head (~164K trainable parameters), plus a separate reproducible retraining module under `training/`.
- **Telemetry & WebSockets**: Low-latency video stream pipeline with MJPEG feed and WebSocket channels for location-scoped emergency telemetry.
- **Stack**: Python 3.10+, FastAPI, OpenCV, MobileNetV2-based CNN (TensorFlow), SQLite, WebSockets.

---

## 🔬 Research & Internship Experience

- **Research Intern — National Institute of Technology (NIT), Kurukshetra**
  - Researched Computer Vision and Machine Learning algorithms for multimodal feature extraction, optical flow motion analysis, and audio signal processing.
  - Built the initial research prototype in Python/Flask that laid the algorithmic foundation for the AI Virality Predictor.

---

## 📈 Computer Science Fundamentals & Practices

- Actively practicing Data Structures & Algorithms (Arrays, Hash Tables, Trees, Graphs, Dynamic Programming, Two Pointers).
- Object-Oriented Design (SOLID principles, Factory, Strategy, and Singleton design patterns).
- Relational database schema design, indexing, transactions (ACID properties), and SQL optimization.

---

## 📫 Let's Connect

- **LinkedIn**: [linkedin.com/in/angel-mishra-992474345](https://www.linkedin.com/in/angel-mishra-992474345/)
- **GitHub**: [github.com/123angmish](https://github.com/123angmish)