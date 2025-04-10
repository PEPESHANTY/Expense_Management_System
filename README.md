# 💸 Expense Management System

A modern and interactive full-stack Expense Management System built with **Streamlit** for the frontend and **FastAPI + MySQL** on the backend.

This app allows users to:
- Add & update daily expenses
- View analytics by category
- Visualize trends month-wise using bar and pie charts


A modern and interactive full-stack Expense Management System built using **Streamlit** for the frontend, **FastAPI** for the backend, and **MySQL** as the database. This app enables users to log daily expenses, track spending patterns, and visualize analytics — all in a beautiful and user-friendly interface.

🔗 **Live App**: [ems-by-shantanu-bhute.streamlit.app](https://ems-by-shantanu-bhute.streamlit.app)  
📦 **GitHub Repo**: [github.com/PEPESHANTY/Expense_Management_System](https://github.com/PEPESHANTY/Expense_Management_System)

---

## 🚀 Features

- 🔥 **Live Animated UI** with gradient transitions
- 🧾 Add and update daily expense entries
- 📊 Visualize expense data by **category** and **month**
- 📅 View expenses for a selected date
- 📉 Generate insightful bar & pie charts
- 🔐 Secure API and DB communication using `.env` files
- 📁 Clean separation of **frontend**, **backend**, and **tests**

---

## 🛠 Tech Stack

| Layer      | Technology                          |
|------------|--------------------------------------|
| Frontend   | [Streamlit](https://streamlit.io)   |
| Backend    | [FastAPI](https://fastapi.tiangolo.com) |
| Database   | MySQL (hosted on a cloud server)     |
| Styling    | HTML + Custom CSS                   |
| Hosting    | Frontend: [Streamlit Cloud](https://streamlit.io/cloud)  
|            | Backend: [Render.com](https://render.com)  

---

## 🌐 Architecture Overview

[Frontend - Streamlit Web App] <=====> [Backend - FastAPI API] <=====> [MySQL Server (Cloud Hosted)] hosted on Streamlit hosted on Render.com hosted on remote server


## 📁 Project Structure

PROJECT_2/ ├── backend/ # 💡 FastAPI backend service │ ├── db_helper.py # Manages database connections (DEV/PROD) │ ├── logging_setup.py # Custom logging configuration for backend │ ├── server.py # Main FastAPI app with API endpoints │ ├── test_api.py # Manual endpoint testing (optional) │ └── .env # Contains environment-based DB config variables │ ├── frontend/ # 🌐 Streamlit frontend app │ ├── app.py # Main app entry point + layout setup │ ├── analytics_ui.py # UI to visualize category-wise spending │ ├── analytics_by_month.py # UI for month-wise charts and analytics │ ├── add_update_ui.py # UI to add or update expenses │ └── .env # Contains ENV setting and PROD API URL │ ├── tests/ # 🧪 Test suite │ └── backend/ │ ├── test_db_helper.py # Unit tests for DB helper functions │ └── conftest.py # Test fixtures setup (e.g., mock connections) │ ├── requirements.txt # Shared dependencies for backend/frontend ├── run_app.bat # Shortcut to run backend & frontend locally (Windows) └── README.md # Project overview, setup guide, and deployment notes

## 🧪 Running Locally

Make sure you have Python 3.10+ installed.

### 1️⃣ Start the Backend API (FastAPI)
```bash
cd backend
uvicorn server:app --reload
```

### 2️⃣ Start the Frontend App (Streamlit)
```bash
cd frontend
streamlit run app.py
```

✅ Deployment
Frontend: Deployed to Streamlit Cloud
Uses the .env to switch between localhost and Render API based on environment.

Backend: Deployed to Render.com
Automatically connects to a remote MySQL server using secure .env credentials.

🙌 Credits
- **Shivam Chaudhary** — for guiding me through setting up the deployment environment.

- **Dhaval Patel** (Codebasics) — for the amazing Python for Data Professionals playlist that helped shape the backend structure and workflow of this project.

👨‍💻 Author
Built with ❤️ by **Shantanu Bhute**
Feel free to fork, improve, and contribute!

