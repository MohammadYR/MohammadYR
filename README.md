## Hi there 👋
<h1 align="center">Hi, I'm Mohammad YR — Backend Engineer (Python/Django)</h1>

<p align="center">
I build clean, testable APIs with Django & DRF, ship with Docker, and scale background jobs with Celery/Redis.
</p>

<p align="center">
<a href="https://github.com/MohammadYR?tab=repositories"><img src="https://img.shields.io/badge/Focus-Django%20%7C%20DRF%20%7C%20Docker%20%7C%20Celery-1"/></a>
<a href="mailto:you@example.com"><img src="https://img.shields.io/badge/Contact-Email-informational"/></a>
</p>
name: Django CI

on:
  push:
    branches: [ "main" ]
  pull_request:
    branches: [ "main" ]

jobs:
  build:

    runs-on: ubuntu-latest
    strategy:
      max-parallel: 4
      matrix:
        python-version: [3.7, 3.8, 3.9]

    steps:
    - uses: actions/checkout@v4
    - name: Set up Python ${{ matrix.python-version }}
      uses: actions/setup-python@v3
      with:
        python-version: ${{ matrix.python-version }}
    - name: Install Dependencies
      run: |
        python -m pip install --upgrade pip
        pip install -r requirements.txt
    - name: Run Tests
      run: |
        python manage.py test
### مهارت‌ها
- RESTful APIs • JWT/OTP • PostgreSQL • Redis
- Celery (retry/backoff/chain) • Caching • Pytest • GitHub Actions
- Git تمیز: Conventional Commits، PRهای کوچک، Releases با SemVer

### پروژه‌های شاخص
- **Custom Shop Project (Django/DRF)** — احراز هویت JWT/OTP، سبد خرید، سفارش‌ها، Docker، Celery/Redis. [Repo](https://github.com/MohammadYR/Custom-Shop-Project)
- **Celery Patterns Pack** — مثال‌های تولیدی برای هندل خطا/Retry/Chain. (به‌زودی)

### ارزش‌ها
Reliability over hype • مستندسازی آموزنده • انتشارهای کوچک و مداوم

<!--
**MohammadYR/MohammadYR** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
