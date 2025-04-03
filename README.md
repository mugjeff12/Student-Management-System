# 🎓 Student Management System (PyQt6 + SQLite)

A full-featured **Student Management System** built using **PyQt6** and **SQLite**.  
It allows you to **insert**, **edit**, **delete**, and **search** student records with a responsive GUI interface. Built for learning GUI development, SQL integration, and application structure.

---

## 🚀 Features

- ➕ Add new student records
- 🔍 Search student by name
- ✏️ Edit existing records
- ❌ Delete records with confirmation
- 📋 View all data in a dynamic table
- 🧠 Uses multi-window dialogs for each operation
- 💾 Connects to an SQLite database
- 🪟 Built entirely with PyQt6

---

## 🧰 Tech Stack

| Technology | Purpose                  |
|------------|--------------------------|
| PyQt6      | GUI framework             |
| SQLite3    | Local database storage    |
| Python     | Core logic & app control |

---

## 🖥️ Interface Preview

*(Add screenshots if you want)*  
> Main Window → Table of students  
> Dialog Boxes → For Insert, Edit, Delete, and Search

---

## 📁 Project Structure

```
StudentManagementSystem/
├── main.py                # Full app code (your script)
├── database.db            # SQLite DB file (created on run)
├── icons/                 # Add icons like add.png, search.png
├── README.md              # This file
```

---

## 💻 How to Run

1. **Install Dependencies**

```bash
pip install PyQt6
```

2. **Run the Application**

```bash
python main.py
```

> The SQLite database (`database.db`) is auto-created on first run.

---

## 🧠 How It Works

- On launch, it loads student data from `database.db` into a table.
- Menubar and toolbar provide access to all actions:
  - Insert new students
  - Search students by name
  - Edit and Delete selected records
- Uses QDialog windows for smooth multi-step interactions.
- Uses `QMessageBox` for about/info and confirmations.

---

## ✅ Database Schema

Table: `students`

| Column | Type    |
|--------|---------|
| id     | INTEGER PRIMARY KEY AUTOINCREMENT |
| name   | TEXT    |
| course | TEXT    |
| mobile | TEXT    |

> Automatically handled on insert.

---

## ✨ To Customize

- Add more fields like email, address, DOB, etc.
- Add input validation (e.g., number format for mobile)
- Add table sorting, search filters, or export to CSV

---

## 👨‍💻 Author

Created by **Mugdho Jeferson Rozario**  
> Engineering Physics @ McMaster | GUI + SQL Enthusiast | Python Dev  
> [GitHub](https://github.com/mugjeff12)

---

## 📜 License

MIT License — free to use, modify, and distribute with credit.

---

## 💡 Tips

- Make sure to add required icons in an `icons/` folder:
  - `add.png` for Add Student
  - `search.png` for Search
- You can remove the `from idlelib.help_about import AboutDialog` line safely — it's not used.

