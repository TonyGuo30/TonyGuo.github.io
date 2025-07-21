---
title: "Employment‑Access WeChat Mini‑Program for People with Disabilities"
excerpt: >
  Cloud‑database–powered WeChat mini‑program that connects **job‑seeking people with disabilities** to **companies & social‑welfare recruiters**.
collection: portfolio
permalink: /portfolio/employment-miniprogram-disabled
header:
  teaser:"disabled-employment-cover.jpg"
---

![Employment‑Access Mini‑Program]({{ '/images/disabled-employment-cover.jpg' | relative_url }})

### Overview
This project tackles the **employment gap faced by people with disabilities** in China by providing an easy‑to‑use **WeChat mini‑program** backed by a cloud database.  
Users are split into two roles:

1. **Recruiters** – companies or social‑welfare organisations who publish inclusive job posts.  
2. **Job‑seekers** – people with disabilities searching, filtering and applying for opportunities.

The mini‑program is **fully copyrighted** and is being rolled out through local communities and the Disabled Persons’ Federation.

---

### Core Features

| Feature | Description |
|---------|-------------|
| **Role‑based login** | Distinct onboarding flows for recruiters vs. job‑seekers. |
| **Cloud database backend** | Real‑time CRUD operations on job posts, user profiles and applications. |
| **Inclusive UX** | Large tappable targets, high‑contrast colour palette, screen‑reader labels. |
| **Questionnaire module** | In‑app survey gathers usability feedback to iteratively improve accessibility. |
| **Application tracking** | Recruiters manage candidate status; job‑seekers receive push notifications. |

---

### Architecture

| Layer | Tech | Purpose |
|-------|------|---------|
| **Frontend** | WeChat mini‑program (WXML / WXSS / JavaScript) | Lightweight client with native WeChat components. |
| **Backend** | Tencent Cloud Database (TCB) | Stores users, job posts, applications, survey results. |
| **Auth & Roles** | WeChat Cloud Functions | Validates openid, assigns recruiter / job‑seeker permissions. |
| **Analytics** | Cloud Functions + TCB logs | Tracks engagement metrics & questionnaire responses. |

---

### Impact
> **Goal:** Increase inclusive employment placements by **≥ 25 %** in participating communities within 12 months.

| Metric | Baseline | Target (12 mo) |
|--------|----------|----------------|
| Registered job‑seekers | 0 | 2 000+ |
| Active recruiter orgs | 0 | 150+ |
| Successful hires | 0 | 500+ |

---

### Acknowledgements
Special thanks to community volunteers, pilot companies, and the **Disabled Persons’ Federation** for continuous feedback and outreach support.

---
