# HelpDesk-AI

A simple and efficient AI-powered Helpdesk system where users can register complaints, track their status, and get automated assistance. This project integrates Google's **Gemini Flash** model to assist in handling user queries and issues.

---

## Project Structure

```text
HelpDesk-AI/
│
├── backend/
│   └── app/
│       ├── apis/
│       ├── core/
│       ├── gemini/
│       ├── models/
│       ├── mongodb/
│       └── main.py
│
├── frontend/
│   ├── images/
│   └── streamlit_ui.py
│
├── .env
├── LICENSE
├── pyproject.toml
├── README.md
```

---

## Features

* Register user complaints
* Track and check the status of complaints
* AI agent built with **Gemini Flash** to assist user interactions
* MongoDB backend for persistent storage
* FastAPI backend
* Streamlit frontend for simple, user-friendly UI

---

## Setup Instructions

> Make sure Python 3.10+ is installed and accessible via `py` or `python3`.

### 1. Clone the repository

```bash
git clone <your-repo-url>
cd HelpDesk-AI
```

### 2. Setup Virtual Environment

```bash
# Create virtual environment
python -m venv .venv

# Activate virtual environment
# Windows
.venv\Scripts\activate

# Unix/MacOS
source .venv/bin/activate
```

### 3. Install Dependencies

Make sure you have [**uv**](https://github.com/astral-sh/uv) installed.

```bash
uv sync
```

### 4. Run the Backend Server

```bash
py -m uvicorn backend.app.main:app --reload
```

### 5. Run the Frontend UI

```bash
py -m streamlit run frontend/streamlit_ui.py
```

---

## Environment Variables

Create a `.env` file in the root directory with the following example:

```env
# Mongo DB
MONGODB_HOST_TEST="localhost"
MONGODB_PORT_TEST="27017"
MONGODB_DATABASE_NAME_TEST="grievances"


# Gemini
GEMINI_API_Key_TEST = "str"
GEMINI_MODEL_NAME_FLASH_TEST = "gemini-2.0-flash"
```

---

## Powered By

* [Gemini Flash (Google GenAI)](https://ai.google.dev/)
* [FastAPI](https://fastapi.tiangolo.com/)
* [Streamlit](https://streamlit.io/)
* [MongoDB](https://www.mongodb.com/)
* [uv (fast dependency manager)](https://github.com/astral-sh/uv)
