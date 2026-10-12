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

## 🎯 Vision & Purpose
As my first personal project, I wanted to keep things straightforward and get a real, hands-on feel for the full-stack development process. 

To be honest, over the summer, days started blurring together where it felt like I did basically nothing. A basic phone trackers would just throw a generic warning saying "X hours = bad," which didn't help me differentiate between spending two hours reading the news or two hours unthinkingly doom-scrolling.

I built ScreenScore to change that narrative. It’s a tool designed to give me a way to quantitatively compare how my days actually stacked up.

### What it does:
* **Weighted Scoring:** Instead of a flat minute-count, it calculates a score from 0 to 100 based on the "Quality Grade" you assign to different categories.
* **Category Context:** Differentiates between a high-value 2-hour coding session and a low-value 2-hour rabbit hole.
* **Trend Tracking:** Visualizes weekly progress so you can instantly spot your productive peaks and dips.
* **Data Persistence:** Backed by Flask and SQLAlchemy to keep a permanent, structured log of your digital habits.



---




## 🛠️ The Tech Stack

* **Backend:** Python with Flask & SQLAlchemy 
* **Frontend:** React + Vite
* **Visualization:** Chart.js to turn raw database entries into visual trends.

---

## 📁 Project Architecture

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

