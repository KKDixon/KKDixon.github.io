---
title: "Screenscore: Screen Time Quality Tracker"
date: 2026-01-03 15:00:00 +0000
categories: [Personal Projects]
tags: [Python, Flask, JS, SQLite, React, Chart.js]
description: A full-stack web application that evaluates the quality of screen time, not just the quantity
image:
  path: ../assets/imgs/screenscore_dashboard.png
  alt: View of the application UI.
---


## 🎯 The Vision
Most screen-time trackers focus on *quantity*—how many hours you spent staring at a glass rectangle. **ScreenScore** flips the script by focusing on **quality**. 

As someone new to web devolopment, I wanted to build a tool that didn't just nag me about my phone usage, but helped me prioritize "Work" and "Learning" over mindless scrolling. I built this using a **Flask** backend and a **React** frontend to get hands-on experience with modern full-stack architecture.

---

## 💡 Purpose & Functionality
The core purpose of ScreenScore is to move beyond the "Screen Time is Bad" narrative and focus on **intentionality**. 

### What it does:
* **Weighted Scoring:** Instead of a flat minute-count, it calculates a score from 0-100 based on the "Quality Grade" you assign to categories.
* **Category Context:** It differentiates between a 2-hour coding session (High Quality) and a 2-hour doom-scroll (Low Quality).
* **Trend Tracking:** It visualizes your progress over the week, helping you identify which days of the week your productivity dips.
* **Data Persistence:** Using a Flask/SQLAlchemy backend, it keeps a permanent record of your digital habits.

---




## 🛠️ The Tech Stack
This project allowed me to bridge the gap between two powerful ecosystems:
* **Backend:** Python with Flask & SQLAlchemy (SQLite for data persistence).
* **Frontend:** React 18 powered by Vite for a lightning-fast UI.
* **Visualization:** Chart.js to turn raw database entries into actionable trends.

---

## 📁 Project Architecture
I organized the project into a clear separation of concerns, ensuring the API logic remains independent of the UI components.

```text
screenscore/
├── backend/
│   ├── app/
│   │   ├── models/        # SQLAlchemy Database models
│   │   ├── routes/        # API Endpoints (CRUD & Analytics)
│   │   └── services/      # Core business & scoring logic
│   └── run.py             # Flask entry point
├── frontend/
│   ├── src/
│   │   ├── pages/         # Dashboard, Sessions, Analytics
│   │   ├── services/      # Axios API integration
│   │   └── utils/         # Score & Date calculation helpers
└── README.md
```

