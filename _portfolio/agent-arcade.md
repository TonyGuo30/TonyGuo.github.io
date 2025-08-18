---
title: "Agent Arcade — Crowd Simulation & Rumor Diffusion Sandbox"
collection: portfolio
permalink: /portfolio/agent-arcade
excerpt: >
  Browser-based **crowd simulation** where tiny agents wander, chat, and spread a **rumor**—with live **analytics**, **replay scrubber**, and **director events** (concert / rain / market).
header:
  teaser: "agent-arcade-cover.jpg"
---

![Agent Arcade — Crowd Simulation]({{ '/images/agent-arcade-cover.jpg' | relative_url }})

### Overview
**Agent Arcade** is an interactive sandbox that visualizes how information spreads through a crowd. Dozens of agents roam a 2D world; when they get close, they **talk**, sometimes **pass along a rumor**, and their **mood** shifts. You can steer the world with one-click **director events** (concert / rain / market), **record** a run, and scrub through the replay while watching live analytics.

---

### Core Features

| Feature | What it does |
|---|---|
| **Rumor diffusion** | Conversations can spread a “rumor” state between agents; probabilities change with events & faction bias. |
| **Director events** | **Concert** pulls agents toward a stage; **Rain** slows movement & dips mood; **Market Day** boosts social mixing. |
| **Replay & scrubber** | Records snapshots every ~200 ms. Enter replay, scrub frames, or auto-play; **bookmarks** jump to key moments. |
| **Dialog bubbles** | Lightweight “LLM-style” text bubbles react to event, faction, rumor, and mood (no API key needed). |
| **Screenshot** | One-click PNG export of the current canvas for shareable stills. |

---

### Analytics & Visualization

| Panel | Insight |
|---|---|
| **Sparklines** | Live trends for **Average Mood (−1..+1)**, **Rumor Count**, **Conversations/min** (rolling). |
| **Minimap: Movement Heat** | Grid heatmap of where agents traveled—reveals hot zones / chokepoints. |
| **Minimap: Diffusion (First-Heard)** | Per-cell “first time rumor appeared” (newer cells glow stronger) → visible **wavefront**. |
| **Bookmarks** | Auto “Peak rumor: N” and “Biggest cluster moment” captured during recording; one-click replay jump. |

---

### Interaction Cheatsheet
- **Play / Pause**, **Speed** (1×/2×/4×)  
- **Drop Gossip** (seed the rumor), **Bias** slider (same-faction chat likelihood)  
- **Director Events:** 🎵 Concert · 🌧️ Rain · 🛒 Market Day  
- **Replay:** Record / Stop / Clear · Enter/Exit Replay · Play/Pause · Scrubber + **Bookmarks**  
- **📸 Screenshot**: saves a PNG

---

### Architecture

| Layer | Tech | Purpose |
|---|---|---|
| **Frontend** | **React + Vite + TypeScript** | UI, controls, analytics panel, minimap, sparklines. |
| **Simulation** | **Phaser 3 (Arcade Physics)** | Agent movement, conversations, rumor spread, events. |
| **State** | **Zustand** | Stats, histories, overlay mode, replay state. |
| **Graphics** | Canvas (Phaser + 2D API) | Main scene + minimap/overlays + screenshots. |

---

### How it Works (brief)
- Each agent has `mood`, `faction A/B/C`, `rumor?`, `influence`.  
- When two agents are within proximity, they may **Converse**. If exactly one has the rumor, it may **transfer**. Mood nudges up/down based on faction affinity and current event.  
- Every ~200 ms the sim **records** positions & states; **bookmarks** are added on peaks/cluster spikes.

---

### Demo

- **Demo:** *[The GitHub repo for this project](https://github.com/TonyGuo30/agent-arcade)*

---

### Status & Next Ideas
- Current: analytics focus (sparklines, diffusion map, bookmarks, replay).  
- Possible next steps: **clip recorder (WebM)** for shareable videos, **new director events** (parade / blackout), or plug in a **real LLM** for richer dialogue.
