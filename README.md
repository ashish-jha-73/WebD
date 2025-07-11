# 📝 Task Manager Web App

A full-stack application using React (frontend) and Django + SQLite (backend).

---

## ⚙️ Getting Started

```bash
# 1. Clone the repo
git clone https://github.com/ashish-jha-73/WebD.git
cd WebD

# 2. Backend setup (Django + SQLite)
cd backend
python3 -m venv venv                # create venv
source venv/bin/activate            # activate it
pip install -r requirements.txt     # install deps
python manage.py makemigrations     # prepare migrations
python manage.py migrate            # apply migrations
# CORS: open backend/settings.py and add:
#   CORS_ALLOWED_ORIGINS = ["http://localhost:5173"]
python manage.py runserver          # start backend at http://127.0.0.1:8000

# 3. Frontend setup (React) – open a NEW terminal
cd ../frontend
npm install                         # install deps
npm run dev                         # start frontend at http://localhost:5173
