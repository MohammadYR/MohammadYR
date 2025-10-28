<h1 align="center">Hi, I'm Mohammad Yousefi — Backend Developer (Python/Django)</h1>

<p align="center">
I build clean, testable APIs with Django & DRF, ship with Docker, and scale background jobs with Celery/Redis.
</p>

<p align="center">
<a href="https://github.com/MohammadYR?tab=repositories"><img src="https://img.shields.io/badge/Focus-Django%20%7C%20DRF%20%7C%20Docker%20%7C%20Celery-green"/></a>
<a href="mailto:your.email@example.com"><img src="https://img.shields.io/badge/Contact-Email-blue"/></a>
</p>

---

### 🚀 مهارت‌ها
- Django / Django REST Framework  
- PostgreSQL / Redis  
- Celery (Tasks, Retries, Chains)  
- Docker / Docker Compose  
- Testing: pytest / coverage  
- CI/CD: GitHub Actions  
- Git تمیز (Conventional Commits, PRها، Releases)

---

### 🧩 پروژه‌های شاخص
#### 🛒 [Custom-Shop-Project](https://github.com/MohammadYR/Custom-Shop-Project)
بک‌اند فروشگاهی کامل با JWT/OTP، Docker، Celery/Redis و API Docs.  
**Tech Stack:** Django, DRF, PostgreSQL, Redis, Celery, Docker, Pytest

#### ⚙️ Celery Patterns Pack *(به‌زودی)*
الگوهای حرفه‌ای برای تسک‌ها، retries، و signal handling در Celery.

---

### 🧠 Architecture (نمونه تصویری)
```mermaid
flowchart LR
  Client -->|HTTPS/JSON| Django[Backend: Django + DRF]
  Django --> Postgres[(Database: PostgreSQL)]
  Django --> Redis[(Cache & Broker)]
  Django -.enqueue.-> Celery[Celery Workers]
  Celery --> Redis
  Celery --> External[(Email / Payment)]
