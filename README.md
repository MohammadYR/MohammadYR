<h1 align="center">Hi, I'm Mohammad Yousefi — Backend Developer (Python/Django)</h1>

<p align="center">
I build clean, testable APIs with Django & DRF, ship with Docker, and scale background jobs with Celery/Redis.
</p>

<p align="center">
<a href="https://github.com/MohammadYR?tab=repositories"><img src="https://img.shields.io/badge/Focus-Django%20%7C%20DRF%20%7C%20Docker%20%7C%20Celery-1"/></a>
<a href="mailto:you@example.com"><img src="https://img.shields.io/badge/Contact-Email-informational"/></a>
</p>

### مهارت‌ها
- RESTful APIs • JWT/OTP • PostgreSQL • Redis
- Celery (retry/backoff/chain) • Caching • Pytest • GitHub Actions
- Git تمیز: Conventional Commits، PRهای کوچک، Releases با SemVer

### پروژه‌های شاخص
- **Custom Shop Project (Django/DRF)** — احراز هویت JWT/OTP، سبد خرید، سفارش‌ها، Docker، Celery/Redis. [Repo](https://github.com/MohammadYR/Custom-Shop-Project)
- **Celery Patterns Pack** — مثال‌های تولیدی برای هندل خطا/Retry/Chain. (به‌زودی)

### ارزش‌ها
Reliability over hype • مستندسازی آموزنده • انتشارهای کوچک و مداوم

### 🧠 Architecture (نمونه تصویری)
```mermaid
flowchart LR
  Client -->|HTTPS/JSON| Django[Backend: Django + DRF]
  Django --> Postgres[(Database: PostgreSQL)]
  Django --> Redis[(Cache & Broker)]
  Django -.enqueue.-> Celery[Celery Workers]
  Celery --> Redis
  Celery --> External[(Email / Payment)]
