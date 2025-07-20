---
title: "Employment‑Access WeChat Mini‑Program for People with Disabilities"
thumb: /images/disabled-employment-cover.jpg
excerpt: >
  Cloud‑database–powered WeChat mini‑program that connects **job‑seeking people with disabilities** to **companies & social‑welfare recruiters**.<br/>
  <img src="{{ '/images/disabled-employment-cover.jpg' | relative_url }}" alt="Mini‑program screenshot" style="max-width:260px;border-radius:8px;">
collection: portfolio
permalink: /portfolio/employment-miniprogram-disabled
keywords: [cloud-database, wechat-mini-program, accessibility, hci, social-impact]
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

### Deployment & Outreach
- **Pilot communities:** Partnered with local disability service centres to distribute QR codes.  
- **Federation support:** Working with the Disabled Persons’ Federation to onboard larger user cohorts.  
- **Copyright:** Mini‑program software copyright filing submitted (ref ID: XYZ‑2025‑07).

---

### Impact
> **Goal:** Increase inclusive employment placements by **≥ 25 %** in participating communities within 12 months.

| Metric | Baseline | Target (12 mo) |
|--------|----------|----------------|
| Registered job‑seekers | 0 | 2 000+ |
| Active recruiter orgs | 0 | 150+ |
| Successful hires | 0 | 500+ |

---

### Next Steps
1. **Accessibility testing** with low‑vision and motor‑impairment users.  
2. **API hardening** to integrate third‑party assistive technologies.  
3. **Scalable cron jobs** for daily digest messages & job‑match recommendations.

---
