# Vivek Kumar Verma
**Backend Software Engineer | Cloud Architecture | Web Security**

📍 Mumbai, India

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=flat-square&logo=linkedin&logoColor=white)](https://linkedin.com/in/vivek-kumar-verma-swe)
[![Email](https://img.shields.io/badge/Email-D14836?style=flat-square&logo=gmail&logoColor=white)](mailto:vivekkumarv273@gmail.com)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=flat-square&logo=github&logoColor=white)](https://github.com/Vivekkumarv123)

Backend-focused engineer building secure, modular APIs and cloud-deployed systems. Engineering philosophy centers on distributed systems design, OWASP-aligned vulnerability mitigation, and infrastructure that moves cleanly from local dev to production. Actively seeking full-time SWE roles.

---

## Achievements

- **Gen AI Elite Club (Top 75) & Top 10 Team — Google Cloud Gen AI Academy APAC** *(Aug 2026)*
  Selected into the Elite Club; placed Top 10 of the Cohort 2 hackathon applying Google Cloud GenAI to a market-ready solution.
- **National Top 100 (#62) — Google Cloud Code Vipassana S15** *(Jun 2026)*
  Ranked 62nd nationwide on cloud architecture and GCP deployment challenges.
- **2nd Runner-Up (3rd Place) — TechSprint AI Hackathon '25** *(Jan 2026)*
  Secured 3rd place out of competing teams at the GDG On Campus (Pillai College of Engineering) hackathon, focused on building impactful, cutting-edge AI solutions.
---

## Technical Arsenal

**Languages**
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![Java](https://img.shields.io/badge/Java-ED8B00?style=flat-square&logo=openjdk&logoColor=white)

**Backend & APIs**
![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=node.js&logoColor=white)
![Express](https://img.shields.io/badge/Express-000000?style=flat-square&logo=express&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)

**Cloud & Infra**
![AWS](https://img.shields.io/badge/AWS-232F3E?style=flat-square&logo=amazonaws&logoColor=white)
![GCP](https://img.shields.io/badge/GCP-4285F4?style=flat-square&logo=googlecloud&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black)

**Databases**
![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=flat-square&logo=mongodb&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white)

**Security & Auth**
`XSS/SQLi Prevention` `JWT/JWE` `OAuth 2.0` `RBAC` `Input Validation`

---

## Architectural Projects

### [DevSec Buddy](https://github.com/Vivekkumarv123/devsec-buddy) — Modular Web Security Scanner
Local vulnerability scanner detecting XSS, SQL injection, and insecure HTTP headers.
- **Architecture:** Decoupled system — Python CLI as the scanning engine, Node.js/Express API for orchestration and result aggregation, Dockerized for consistent cross-platform runs.
- **Performance:** Async scan orchestration runs progressive checks (Basic → Standard → Deep) without blocking the event loop, cutting full-scan time from **[baseline]s to [Xs]** on a **[N]-file** test target. *← replace with your actual benchmark numbers*
- **Design decision:** Chose a CLI-to-API split over a monolith so the scan engine can run standalone in CI pipelines independent of the dashboard.

### [Legal Advisor](https://github.com/Vivekkumarv123/legal-advisor) — AI-Assisted Legal Document Pipeline
Multi-stage NLP pipeline that turns legal documents into plain-language summaries.
- **Pipeline:** OCR → text extraction → clause identification → AI summarization, processing documents averaging **[N] pages** in **[X] seconds** end-to-end. *← replace with real measured numbers*
- **Security:** Zero-persistence design — documents are processed in memory and never written to disk post-analysis, with validated/sanitized upload handling for sensitive legal text.
- **Design decision:** Chose a multi-stage pipeline over a single LLM call to keep clause extraction auditable and debuggable independent of the summarization step.

### [DevDrop](https://github.com/Vivekkumarv123/DevDrop) — Developer Resource Discovery Platform
Community-driven platform for sharing and discovering curated dev resources.
- **Data model:** MongoDB with strategic indexing on tag fields; SQLite used for local caching to reduce redundant lookups.
- **Access control:** Middleware-based RBAC with JWT auth gating moderation actions.
- **Scale:** *[Add real numbers if you have them — e.g. "indexed search over N resources, median query time Xms" — or drop this line entirely if the platform hasn't been load-tested yet. An honest "architected for scale, not yet load-tested" beats an invented number.]*

### [axios-smart-client](https://github.com/Vivekkumarv123/axios-smart-client) — Enhanced HTTP Client Library
Wrapper around Axios eliminating boilerplate for auth, retries, and error handling.
- **Design:** Singleton client instance; automatic token refresh; exponential-backoff retry (configurable for network/5xx/timeout failures); normalized error responses across all failure modes.
- **Design decision:** Interceptor-based approach chosen so consuming apps get retry/auth logic with zero call-site changes.
  
---

Open to discussing distributed systems, web security, full-time SWE opportunities, open source contributions, or freelance work — links are up top.
