# Expense Tracker Frontend

## Project Overview

This is the frontend application for the Expense Tracker project developed using Streamlit.

The application connects with the FastAPI backend server and allows users to:

* Add Expenses
* View Expenses
* Update Expenses
* Delete Expenses
* View Expense Summary

---

# Tech Stack

* Python
* Streamlit
* Pandas
* Requests

---

# Features

## Add Expense

Users can add:

* Title
* Amount
* Category
* Payment Method
* Expense Date
* Description

## View Expenses

Displays all expenses in table format.

## Update Expense

Allows updating existing expense details.

## Delete Expense

Delete expenses using Expense ID.

## Expense Summary

Displays category-wise expense analysis with charts.

---

# Project Structure

```bash
frontend/
│
├── ft.py
├── requirements.txt
└── .streamlit/
    └── secrets.toml
```

---

# Installation

## Step 1: Clone Repository

```bash
git clone <repository_url>
```

---

## Step 2: Navigate to Frontend Folder

```bash
cd frontend
```

---

## Step 3: Install Dependencies

```bash
pip install -r requirements.txt
```

---

# requirements.txt

```txt
streamlit
requests
pandas
```

---

# Configure Backend URL

Create folder:

```bash
.streamlit
```

Inside it create:

```bash
secrets.toml
```

Add:

```toml
be_server_url = "http://127.0.0.1:8000"
```

For deployed backend:

```toml
be_server_url = "https://your-backend-url.onrender.com"
```

---

# Run Frontend Locally

```bash
streamlit run ft.py
```

Frontend runs on:

```bash
http://localhost:8501
```

---

# Backend Requirement

Before running frontend, ensure backend server is running.

Example Backend URL:

```bash
http://127.0.0.1:8000
```

---

# Deployment

## Deploy on Streamlit Cloud

### Deployment Steps

1. Push frontend code to GitHub
2. Open Streamlit Cloud
3. Connect GitHub repository
4. Select:

   * Branch
   * frontend/ft.py
5. Add secrets in Streamlit Cloud:

```toml
be_server_url = "https://your-backend-url.onrender.com"
```

6. Deploy Application

---

# Application Screens

* Add Expense
* View Expenses
* Update Expense
* Delete Expense
* Expense Summary Dashboard

---

# Author

Keerthana Reddy

Python Developer | Full Stack Developer
