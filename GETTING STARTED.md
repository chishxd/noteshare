# 📚 NoteShare — Setup Guide

Hey teammate! Follow this exactly — no shortcuts.

---

## ✅ 1️⃣ Install Python

**Windows:**

* Download [Python 3.11+](https://www.python.org/downloads/windows/)
* During setup, ✅ **tick “Add Python to PATH”**

**Linux/macOS:**

* Check if installed: `python3 --version`
* If not, install:

  ```bash
  # macOS
  brew install python

  # Ubuntu/Debian
  sudo apt update && sudo apt install python3 python3-pip
  ```

---

## ✅ 2️⃣ Install Git

**Windows:**

* Download [Git for Windows](https://git-scm.com/download/win)
* During setup:

  * ✅ “Checkout as-is, commit Unix-style line endings”
  * ✅ “Use Git from the command line and also from 3rd-party software”
  * ✅ Use **OpenSSH** (default)

**Linux/macOS:**

* Already installed on most. If not:

  ```bash
  sudo apt install git  # Debian/Ubuntu
  brew install git      # macOS
  ```

---

## ✅ 3️⃣ Set up your SSH key (once)

1. Open **Git Bash** (Windows) or **Terminal** (Linux/macOS):

   ```bash
   ssh-keygen -t ed25519 -C "your_email@example.com"
   ```

   Just press **Enter** 3 times.

2. Show your public key:

   ```bash
   cat ~/.ssh/id_ed25519.pub
   ```

3. Copy that key and add it to GitHub:
   👉 [Add SSH key to GitHub](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/adding-a-new-ssh-key-to-your-github-account)

---

## ✅ 4️⃣ Install Poetry

**Windows (PowerShell):**

```powershell
(Invoke-WebRequest -Uri https://install.python-poetry.org -UseBasicParsing).Content | python -
```

**Linux/macOS:**

```bash
curl -sSL https://install.python-poetry.org | python3 -
```

Verify:

```bash
poetry --version
```

---

## ✅ 5️⃣ Clone the project

```bash
cd path/to/your/projects
git clone git@github.com:chishxd/noteshare.git
cd noteshare
```

---

## ✅ 6️⃣ Keep your `.venv` inside the project

```bash
poetry config virtualenvs.in-project true
```

---

## ✅ 7️⃣ Install dependencies

```bash
poetry install
```

---

## ✅ 8️⃣ Activate your virtual environment

```bash
poetry shell
```

You should see:

```
(.venv) user@pc noteshare $
```

---

## ✅ 9️⃣ Run the project

```bash
python -m noteshare.main
```

---

## ✅ 1️⃣0️⃣ VSCode tips

✅ Open the **project folder** in VSCode.
✅ `Python: Select Interpreter` → choose the one in `.venv`.
✅ VSCode will auto-activate:

```bash
source .venv/bin/activate
# or
source .venv/Scripts/activate  # Windows
```

✅ Run & debug as normal.

---

## ⚡ Common commands

| What?            | Command                          |
| ---------------- | -------------------------------- |
| Update code      | `git pull origin dev`            |
| Install deps     | `poetry install`                 |
| Run scripts      | `poetry shell` → `python -m ...` |
| Add a package    | `poetry add package_name`        |
| Remove a package | `poetry remove package_name`     |
| Run tests        | `poetry run pytest`              |

---

## 💡 Troubleshooting

✅ Always use **PowerShell** or **Git Bash** on Windows — not old CMD.
✅ If you get `permission denied` when pushing, double-check your SSH key.
✅ If VSCode uses the wrong Python, re-select the `.venv` interpreter.

---

You’re all set! 🚀