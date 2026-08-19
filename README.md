# HelpDesk-AI
 

https://github.com/user-attachments/assets/b5d9a3e8-9d80-444e-9123-2bdca5c49562


## ⚙️ Setup Instructions

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

## 🔐 Environment Variables

Create a `.env` file in the root directory with the following (example):

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

## 🧠 Powered By

* [Gemini Flash (Google GenAI)](https://ai.google.dev/)
* [FastAPI](https://fastapi.tiangolo.com/)
* [Streamlit](https://streamlit.io/)
* [MongoDB](https://www.mongodb.com/)
* [uv (fast dependency manager)](https://github.com/astral-sh/uv)

---

## 📌 TODO / Future Improvements

* Add login/authentication system
* Admin dashboard for complaint management
* Notification/email integration for updates
* Improve UI/UX with chat-like interface

---

## 📃 License

This project is licensed under the MIT License - see the [LICENSE](https://chatgpt.com/c/LICENSE) file for details.

---

Let me know if you want me to auto-generate a `README.md` file in your directory structure as well.
