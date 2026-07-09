<div align="center">

# 👋 Amir Zamani | امیر زمانی
### `aka BlackHydra`

**Hardware & Firmware Developer · Financial Markets Programmer · Robotics Engineer**
**برنامه‌نویس سخت‌افزار و بازارهای مالی · مهندس رباتیک**

<img src="https://komarev.com/ghpvc/?username=Amirzamani1l&label=Profile%20Views&color=6a0dad&style=flat" alt="profile views" />
<img src="https://img.shields.io/badge/status-open%20to%20work-brightgreen?style=flat" alt="status" />

</div>

---

## 🧭 About Me / درباره من

> Former Computer Engineering student (dropped out) — 2nd place, **NTE Robotics** · 3rd place, **Robotics Engineering Notebook**
> Delegate at **First Global Challenge 2024 — Athens, Greece 🇬🇷**

- 🤖 I build things that sit at the intersection of **hardware, embedded systems, and software** — from microcontrollers to full-stack platforms.
- 📈 I also design and code **algorithmic trading systems** and do **quantitative analysis** on financial markets.
- 🔐 Interested in networking, security fundamentals, and hardware/software repair for mobile, laptop & PC.
- 🧠 Currently deepening my knowledge of Machine Learning (completed **CS50 AI**) and PCB design.
- 🌍 Competed internationally in robotics (First Global 2024, Athens).

<sub>
دانشجوی سابق مهندسی کامپیوتر (اخراجی) — نفر دوم مسابقات NTE رباتیک، نفر سوم دفترچه مهندسی رباتیک<br/>
عضو تیم اعزامی به مسابقات جهانی <b>First Global Challenge 2024</b> در آتن، یونان 🇬🇷<br/>
چیزهایی می‌سازم که سخت‌افزار، سیستم‌های نهفته (Embedded) و نرم‌افزار رو کنار هم قرار می‌ده — از میکروکنترلر تا پلتفرم‌های فول‌استک.
همچنین سیستم‌های معاملات الگوریتمی طراحی و کدنویسی می‌کنم و روی بازارهای مالی تحلیل کمّی انجام می‌دم.
</sub>

---

## 🛠️ Skills & Technologies / مهارت‌ها

<table>
<tr>
<td valign="top" width="50%">

**🤖 Robotics · IoT · Embedded**
<br/>
<img src="https://img.shields.io/badge/C-A8B9CC?style=for-the-badge&logo=c&logoColor=black"/>
<img src="https://img.shields.io/badge/C++-00599C?style=for-the-badge&logo=cplusplus&logoColor=white"/>
<img src="https://img.shields.io/badge/Arduino-00979D?style=for-the-badge&logo=arduino&logoColor=white"/>
<img src="https://img.shields.io/badge/MicroPython-2B2728?style=for-the-badge&logo=micropython&logoColor=white"/>
<img src="https://img.shields.io/badge/ROS-22314E?style=for-the-badge&logo=ros&logoColor=white"/>
<img src="https://img.shields.io/badge/TinyML-FF6F00?style=for-the-badge&logo=tensorflow&logoColor=white"/>
<img src="https://img.shields.io/badge/PCB%20Design-1A1A1A?style=for-the-badge&logo=kicad&logoColor=white"/>

**💹 Algorithmic Trading · Quant**
<br/>
<img src="https://img.shields.io/badge/Pine%20Script-131722?style=for-the-badge&logo=tradingview&logoColor=white"/>
<img src="https://img.shields.io/badge/MQL4%20%26%205-0B3D91?style=for-the-badge"/>
<img src="https://img.shields.io/badge/Quantitative%20Analysis-004B87?style=for-the-badge"/>
<img src="https://img.shields.io/badge/Crypto%20Bots-F7931A?style=for-the-badge&logo=bitcoin&logoColor=white"/>

</td>
<td valign="top" width="50%">

**💻 Software · AI · Backend**
<br/>
<img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white"/>
<img src="https://img.shields.io/badge/Flask-000000?style=for-the-badge&logo=flask&logoColor=white"/>
<img src="https://img.shields.io/badge/SQLite-07405E?style=for-the-badge&logo=sqlite&logoColor=white"/>
<img src="https://img.shields.io/badge/Machine%20Learning-FF6F00?style=for-the-badge&logo=scikitlearn&logoColor=white"/>
<img src="https://img.shields.io/badge/CS50AI-Certified-1B4F72?style=for-the-badge"/>
<img src="https://img.shields.io/badge/Selenium-43B02A?style=for-the-badge&logo=selenium&logoColor=white"/>

**🔐 Security · Systems · Tools**
<br/>
<img src="https://img.shields.io/badge/Networking-4B0082?style=for-the-badge"/>
<img src="https://img.shields.io/badge/Ducky%20Script-000000?style=for-the-badge"/>
<img src="https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white"/>
<img src="https://img.shields.io/badge/HW%2FSW%20Repair-777777?style=for-the-badge"/>

</td>
</tr>
</table>

---

## 🚀 Featured Project — REOS

**A full-stack Real Estate Operations Platform** (portfolio build — architecture below is generalized, no client/business data included).

REOS is a self-hosted system that turns scattered real-estate listings and leads into a single operational tool: it scrapes and normalizes listings, matches them against buyer/renter profiles, and gives agents an AI assistant and a Telegram bot to work from.

```
┌─────────────┐     ┌──────────────┐     ┌────────────────┐
│  Scraper     │────▶│   SQLite DB   │◀────│   Flask API     │
│  (Selenium)  │     │  (db.py core) │     │   (server.py)   │
└─────────────┘     └──────────────┘     └────────────────┘
                             ▲                     │
              ┌──────────────┼─────────────┐       ▼
              │              │              │  ┌──────────┐
      ┌───────────────┐┌───────────┐┌─────────────┐ Web UI  │
      │ Matching Engine││ AI Agent  ││ Telegram Bot│└──────────┘
      │  (matching.py) ││ (ai.py)   ││(telegram_bot)│
      └───────────────┘└───────────┘└─────────────┘
```

**Core modules & what they do:**

- 🕷️ **`scraper.py`** — Selenium-based crawler that continuously collects and deduplicates listings, verifying each ad's detail page to filter noise before it ever reaches the database.
- 🗄️ **`db.py`** — Single source of truth for all data (listings, clients, advisors, tasks, price history) built on SQLite with WAL mode for safe concurrent access between the scraper and the API.
- 🧮 **`matching.py`** — A standalone, dependency-free scoring engine that ranks listings against client requirements (budget, location, room count, area) and returns a weighted match score with human-readable reasons.
- 🌐 **`server.py`** — A Flask REST API exposing 40+ endpoints: listings, clients, advisors, task auto-assignment, review workflows, and an official third-party marketplace API integration (OAuth + webhooks + quota tracking).
- 🤖 **`telegram_bot.py`** — A Telethon-based userbot that lets an agent manage clients and tasks straight from Telegram, with an AI command built in.
- 🧠 **`ai.py`** — An LLM-backed assistant with two personas: an internal assistant for the agent, and a customer-facing sales persona that only ever talks about real, in-stock listings — no hallucinated data.
- 🛰️ **`sat.py`** — Satellite change-detection module: pulls Sentinel-2 imagery, computes NDVI difference maps with NumPy/PIL, and flags areas with meaningful land-cover change.
- 🖥️ **`console.py`** — A safety-scoped, in-app SQL/command terminal for admins with query whitelisting and report generation.

**Highlights:**
- End-to-end pipeline from raw scraped data → cleaned & verified listings → matched leads → agent action, with almost no manual data entry.
- Defensive DB design: safe cleanup scripts, upsert-based migrations, WAL journaling for concurrent read/write.
- AI integration designed with guardrails (output sanitization, strict "only real inventory" prompting) rather than free-form generation.

---

## 📌 Other Projects / سایر پروژه‌ها

| Project | Stack | Description |
|---|---|---|
| 🎥 **OpenCV Vision Project** | Python, OpenCV | Computer vision utilities & experiments |
| 📈 **Pine Script Strategies** | Pine Script | Custom indicators & trading strategies for TradingView |
| 🤖 **MQL4/5 Expert Advisors** | MQL4/5 | Automated trading logic for MetaTrader |
| 🌐 **Portfolio Website** | HTML/CSS | Personal portfolio site |

---

## 📊 GitHub Stats

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=Amirzamani1l&show_icons=true&theme=radical&hide_border=true" alt="stats" width="48%"/>
  <img src="https://github-readme-streak-stats.herokuapp.com/?user=Amirzamani1l&theme=radical&hide_border=true" alt="streak" width="48%"/>
</p>

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=Amirzamani1l&layout=compact&theme=radical&hide_border=true" alt="top langs" width="48%"/>
  <img src="https://github-readme-activity-graph.vercel.app/graph?username=Amirzamani1l&theme=redical&hide_border=true" alt="activity graph" width="48%"/>
</p>

---

## 🌐 Connect / ارتباط با من

<p align="left">
  <a href="https://instagram.com/amirzamani1l" target="_blank"><img src="https://img.shields.io/badge/Instagram-E4405F?style=for-the-badge&logo=instagram&logoColor=white"/></a>
  <a href="https://hackster.io/amirzamani1l" target="_blank"><img src="https://img.shields.io/badge/Projects-Hackster.io-2E2E2E?style=for-the-badge"/></a>
  <a href="https://www.linkedin.com/in/amir-zamani-1909a8315" target="_blank"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white"/></a>
  <a href="https://t.me/Black_Hydra" target="_blank"><img src="https://img.shields.io/badge/Telegram-2CA5E0?style=for-the-badge&logo=telegram&logoColor=white"/></a>
  <a href="https://t.me/BlackHydra_Chat" target="_blank"><img src="https://img.shields.io/badge/Telegram%20Group-2CA5E0?style=for-the-badge&logo=telegram&logoColor=white"/></a>
  <a href="https://x.com/amirzamani1l" target="_blank"><img src="https://img.shields.io/badge/X-000000?style=for-the-badge&logo=x&logoColor=white"/></a>
  <a href="https://www.threads.net/@amirzamani1l" target="_blank"><img src="https://img.shields.io/badge/Threads-000000?style=for-the-badge&logo=threads&logoColor=white"/></a>
</p>

---

<p align="center"><i>⭐️ From <a href="https://github.com/Amirzamani1l">Amir Zamani (BlackHydra)</a></i></p>
