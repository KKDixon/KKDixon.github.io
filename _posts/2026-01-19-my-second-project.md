---
title: "BookShelf: Personal Library Manager"
date: 2026-01-19 15:00:00 +0000
categories: [Personal Projects]
tags: [Python, JS, Flask, Vite, React, Google Books API]
description: A full-stack web application for managing your personal book collection with a (upcoming) beautiful 3D bookshelf visualization.
image:
  path: ../assets/imgs/bookshelf_dashboard.png
  alt: View of the application UI.
---

## 🎯 The Vision

I wanted to build a space that captured the "antique library" vibe—leather, wood, and quiet focus—while using a modern tech stack to handle the heavy lifting of data entry. This project is a labor of love, combining my interest in full-stack architecture with my passion for reading.

---

## 💡 Purpose & Functionality

The goal was simple: **Less typing, more reading.** I built this to solve the friction of manual entry. By integrating the **Google Books API**, I can add a book to my digital shelf in seconds. The app stores a title and tracks the pulse of my reading habit.

---




## 🛠️ The Tech Stack

I chose this stack to learn how to bridge a robust Python backend with a reactive, modern frontend.

* **Backend:** Python & Flask 3.0. I used **SQLAlchemy** because I wanted to practice proper relational mapping with a SQLite database.
* **Frontend:** React 18 (Vite). I focused on building reusable components and handling asynchronous data with **Axios**.
* **Visualization:** **Recharts** for the data, and custom **CSS3** for that specific antique library aesthetic I was wanted.

---

## 📁 Project Architecture


```text
bookshelf/
├── backend/
│   ├── app/
│   │   ├── models/          # Where the book and user data lives
│   │   ├── routes/          # My REST API endpoints (CRUD & Stats)
│   │   └── __init__.py      # App factory setup
│   ├── run.py               # Entry point
│   └── requirements.txt     
├── frontend/
│   ├── src/
│   │   ├── components/      # Reusable UI like the BookCard and Analytics
│   │   ├── services/        # The Axios bridge to my Flask API
│   │   ├── App.jsx          # Main logic
│   │   └── main.jsx         
└── README.md
```

---