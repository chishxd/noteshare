# 📑 Contributing Guide — NoteShare

Thanks for helping build **NoteShare**!  
Please follow this workflow to keep our code clean and conflict-free.

---

## 🚩 Branch Strategy

✅ **`main`** — Production-ready only. Do **not** commit directly here.  
✅ **`dev`** — Integration branch. All features merge here first.  
✅ **`feature/*`** — Your working branches. Always branch off `dev`.

**Example:**  
```bash
git checkout dev
git pull origin dev
git checkout -b feature/login-page
````

---

## ✅ Commit Style

* Write clear commits: `feat: add login API` or `fix: bug in upload form`
* Use present tense: `add`, `fix`, `update` — not past tense.

---

## ✅ Pull Requests

1. Push your `feature/*` branch to origin.
2. Open a PR **into `dev`** — not `main`.
3. Link related issues in the PR description (`Closes #5`).
4. Keep PRs small and focused. Big PRs will be sent back.

---

## ✅ Keep Up To Date

Before you start new work:

```bash
git checkout dev
git pull origin dev
```

---

## ✅ Testing

* Run `python manage.py makemigrations` & `migrate` if you add models.
* Run the server locally to test new features.
* Don’t commit `.env` or secrets. Always add new secrets to `.gitignore`.

---

## ✅ Issues & Discussions

* Create an **Issue** for any new feature or bug.
* Use the Project Board if needed.
* Assign yourself so work isn’t duplicated.

---

## ⚙️ Good Practices

* Add comments in complex code.
* Keep code style consistent (we use `black` for Python).
* Ask for review if you’re unsure — better early than messy later.

---

## 🤝 Let’s Build It Right

Stick to this — we’ll save hours of merge conflicts and confusion.
Thanks for contributing! 🙌
