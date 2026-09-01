# Angel Mishra

**Java Backend Developer | Full-Stack Software Engineer**  
B.Tech in Electronics & Communication Engineering — **Banasthali Vidyapith**  
*Machine Learning & Computer Vision Research Exposure (NIT Kurukshetra Internship & Final Year Project)*

[![Live Portfolio](https://img.shields.io/badge/🌐_Live_Portfolio-Visit_Website-00C7B7?style=for-the-badge&logo=google-chrome&logoColor=white)](https://123angmish.github.io/angel-mishra-portfolio/)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Angel_Mishra-0A66C2?style=for-the-badge&logo=linkedin)](https://www.linkedin.com/in/angel-mishra-992474345/)
[![GitHub](https://img.shields.io/badge/GitHub-123angmish-181717?style=for-the-badge&logo=github)](https://github.com/123angmish)

---

## 👨‍💻 Professional Summary

I am a software engineer focused on building robust, secure backend systems in **Java & Spring Boot** and dynamic full-stack applications with **React.js / Next.js**. I emphasize writing clean, testable code, enforcing strong authentication & authorization boundaries, designing relational database schemas, and applying efficient Data Structures & Algorithms to solve practical engineering problems.

- 🌐 **Portfolio Website**: [123angmish.github.io/angel-mishra-portfolio](https://123angmish.github.io/angel-mishra-portfolio/)
- 🎯 **Current Focus**: Building secure RESTful APIs, Spring Security authentication architectures, and database concurrency & transaction management.
- 💼 **Target Roles**: Java Backend Developer, Full-Stack Developer, Software Development Engineer (SDE).
- 🧠 **Core CS**: Data Structures & Algorithms, Object-Oriented Programming (OOP), Database Management Systems (DBMS), Operating Systems, Computer Networks.

---

## 🛠️ Technical Stack

| Area | Technologies |
| :--- | :--- |
| **Backend & APIs** | Java 21, Spring Boot (3.x), Spring Security 6, Spring Data JPA, Hibernate, RESTful APIs, JWT, BCrypt, Jakarta Validation |
| **Frontend** | React.js, Next.js, Redux Toolkit, JavaScript (ES6+), TypeScript, HTML5, CSS3, Tailwind CSS, Vite |
| **Databases & ORM** | PostgreSQL, MySQL, H2 Database, Hibernate ORM, Flyway Database Migrations |
| **Tools & Environments** | Git, GitHub, Maven, Docker, Postman, Linux / Bash, MVC Architecture |
| **ML & Computer Vision** | Python 3.10+, FastAPI, OpenCV, MobileNetV2 / TensorFlow, Librosa, Scikit-Learn |

---

## 🌟 Featured Projects

### 🌐 [Interactive Developer Portfolio](https://github.com/123angmish/angel-mishra-portfolio) · [Live Demo](https://123angmish.github.io/angel-mishra-portfolio/)
*Modern developer portfolio website with interactive project showcases, constellation navigation, and full responsiveness.*
- **Features**: Responsive design, constellation interactive nodes, research details, downloadable resume, and static production export.
- **Stack**: Next.js 16, React 19, TypeScript, Tailwind CSS, GitHub Pages.

---

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
- **Computer Vision Pipeline**: Combines a MobileNetV2-based CNN for frame-level flood scene classification with Lucas–Kanade optical flow for relative surface motion tracking and estimated flow analysis.
- **Verified Architecture**: Saved model contains a MobileNetV2-based frozen backbone (~2.26M non-trainable parameters) with a custom dense binary classification head (~164K trainable parameters), plus a separate reproducible retraining module under `training/`.
- **Telemetry & WebSockets**: Low-latency video stream pipeline with MJPEG feed and WebSocket channels for location-scoped emergency telemetry.
- **Stack**: Python 3.10+, FastAPI, OpenCV, MobileNetV2-based CNN (TensorFlow), SQLite, WebSockets.

---

### 5. [Cooknetic AI](https://github.com/123angmish/Cooknetic-AI) — AI Culinary Companion & Smart Kitchen Platform
*Full-Stack AI culinary platform powered by Spring Boot and Google Gemini multimodal vision for fridge-scanning, recipe generation, and voice workflows.*
- **Stack**: Java, Spring Boot, Google Gemini API, Web Speech API.

---

### 6. [BreakChain AI](https://github.com/123angmish/breakchain-AI) — Mental Wellbeing & Recovery Platform
*Empathetic support platform featuring AI-assisted reflection, therapeutic recovery tools, and voice journaling.*
- **Stack**: Java, Maven, Google Gemini, OpenAI, Web Audio API.

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

## 📬 Let's Connect

- **🌐 Live Portfolio**: [123angmish.github.io/angel-mishra-portfolio](https://123angmish.github.io/angel-mishra-portfolio/)
- **📧 Email**: [angelmishraofficial@gmail.com](mailto:angelmishraofficial@gmail.com)
- **💼 LinkedIn**: [linkedin.com/in/angel-mishra-992474345](https://www.linkedin.com/in/angel-mishra-992474345/)
- **🐙 GitHub**: [github.com/123angmish](https://github.com/123angmish)
