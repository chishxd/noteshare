# 📚 NoteShare

**NoteShare** is an open-source study library for students to **upload**, **organize**, and **share** notes, books, and study materials — all in one place.

---

## ✨ Features

- 🔑 **User authentication:** Sign up, log in, manage your profile
- 📂 **Upload & download:** Add your notes (PDFs, images, docs), download shared resources
- 🗂️ **Organize by subjects & topics:** Tag and sort files for easy browsing
- 🔍 **Search & filter:** Find what you need, fast
- 🛡️ **Admin dashboard:** Moderate uploads, manage users

---

## 🛠️ Tech Stack

- **Backend:** Python + Django
- **Frontend:** Django Templates (HTML, CSS — Bootstrap/Tailwind)
- **Database:** SQLite (dev) → PostgreSQL (prod)
- **Storage:** Local file storage (dev) → S3/Cloud storage (prod)
- **Hosting:** [To be decided] (Heroku, Render, or Railway)

---

## ⚙️ Installation

1. **Clone the repo**
   ```bash
   git clone https://github.com/chishxd/noteshare.git
   cd noteshare
   ```

2. **Create a virtual environment**

   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. **Install dependencies**

   ```bash
   pip install -r requirements.txt
   ```

4. **Set up the database**

   ```bash
   python manage.py migrate
   ```

5. **Run the server**

   ```bash
   python manage.py runserver
   ```

6. **Open in your browser**

   ```
   http://127.0.0.1:8000/
   ```

---

## 🚀 Roadmap

* [ ] Basic user auth (signup, login, logout)
* [ ] File upload & storage
* [ ] Subject & topic tagging
* [ ] Search & filters
* [ ] Admin moderation tools
* [ ] Deploy to live server

---

## 🧑‍💻 Contributing

We’re building this together!

* Create an issue for bugs or new features
* Fork the repo, create a branch, open a PR
* Keep commits clean and well-documented

See [CONTRIBUTING.md](CONTRIBUTING.md) for our workflow, branch rules, and PR guidelines.

---

## 📄 License

[MIT License](LICENSE)

---

## 🤝 Authors

* **Chish** — [GitHub](https://github.com/chishxd)
* **Vedant Parte** — [GitHub](https://github.com/VedantParte23)
* **Muinashraf Momin** — [No Github yet]
* **Rihan Jamadar** — [No Github Yet]
---

## ❤️ Acknowledgements

* [Django](https://www.djangoproject.com/)
* [Bootstrap](https://getbootstrap.com/) / [Tailwind CSS](https://tailwindcss.com/)
* Open-source community

---

> *“Built by students, for students — keep learning, keep sharing.”*
