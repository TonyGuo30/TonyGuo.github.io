---
title: "Speech Recognition Trash Can"
excerpt: >
  Voice-activated smart bin with Mandarin command recognition (≈93% accuracy).<br/>
  <img src="{{ '/images/project3.jpg' | relative_url }}" alt="Portfolio preview" style="max-width:260px;border-radius:8px;">
collection: portfolio
permalink: /portfolio/speech-recognition-trash-can

---

![Speech Recognition Trash Can]({{ "/images/project3.jpg" | relative_url }})

### Overview
A **voice-activated disposal system** that opens its lid in response to natural Mandarin commands (e.g., “打开” *open*, “关闭” *close*). The device combines an **HBR640 speech recognition chip** with a microcontroller, Python/MATLAB offline training utilities, and simple on-device keyword classification. The result: **~93% command recognition accuracy** and a ~19% functional improvement (hands-free accessibility & reduced false trigger rate versus baseline IR-only lid systems).

---

### Problem & Motivation
Conventional “automatic” trash cans rely on IR proximity sensors—triggering accidentally (pets, passersby), wasting power, and offering no multi-command interaction (e.g., timed open). The goal was to enable *intent-driven*, hygienic interaction using **low-cost embedded speech recognition** tuned for Mandarin commands without requiring cloud connectivity.

---

### System Architecture

| Layer | Components | Purpose |
|-------|-----------|---------|
| **Audio Front End** | Electret mic -> preamp -> HBR640 | Capture & pre-process audio; on-chip feature frames |
| **Recognition Core** | HBR640 (keyword slots) | On-device isolated word recognition; command ID + confidence |
| **Microcontroller** | (STM32 / Arduino-class MCU) | Serial to HBR640; debounce; confidence filtering; drive actuator |
| **Actuation** | Servo / geared motor + hinge | Open / close dual-flap lid with smooth motion + timeout |
| **Support Scripts** | Python + MATLAB | Dataset augmentation; feature inspection; confusion matrix tuning |

---

### Command Set (Example)

| ID | Mandarin | Pinyin | Action |
|----|----------|--------|--------|
| 1 | 打开 | da kai | Open lid |
| 2 | 关闭 | guan bi | Close lid |
| 3 | 停止 | ting zhi | Halt motion (safety) |
| 4 | 暂停 | zan ting | Pause open timer |
| 5 | 垃圾桶 | la ji tong | Wake / attention (hotword) |
