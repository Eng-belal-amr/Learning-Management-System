# 🎓 EduCenter LMS

A lightweight, fully client-side **Learning Management System** for educational centers. No server, no database, no installation required — just open the HTML file in any browser and start managing your students, courses, and enrollments.

---

## ✨ Features

- 🔐 **Login system** with username & password (3 role levels: Admin, Staff, Viewer)
- 👥 **Student management** — add, search, filter by age group, delete
- 📚 **Course catalog** — categories, age groups, instructor, capacity, fees, status
- 📋 **Enrollments** — link students to courses, track payment status
- 📊 **Reports** — payment summary, expected fees, breakdowns by age group & category
- 💾 **Persistent storage** — all data saved in `localStorage`, survives page refresh
- 📱 **Fully responsive** — works on desktop, tablet, and mobile
- ⚡ **Zero dependencies** — single HTML file, no npm, no build step

---

## 🚀 Live Demo


---

## 🔑 Default Login

| Username | Password  | Role  |
|----------|-----------|-------|
| `admin`  | `admin123`| Admin |

> ⚠️ **Change the default password** immediately after first login via **Settings → User Accounts → Change My Password**.

---

## 📁 Project Structure

```
educenter-lms/
├── lms.html        ← The entire application (open this in a browser)
└── README.md       ← You are here
```

---

## 🖥️ Local Usage

No installation needed:

1. Download `lms.html`
2. Open it in any modern browser (Chrome, Firefox, Edge, Safari)
3. Log in with `admin` / `admin123`
4. Start adding students and courses!

> All data is stored in your browser's `localStorage`. Clearing browser data will erase it — export important records manually if needed.

---

## ☁️ Deploy on GitHub Pages (Free Hosting)

Follow the steps in the [Deployment Guide](#deployment-guide) section below.

---

## 📖 How to Use

### Students
- Go to **Students** → click **+ Add Student**
- Fill in name, age, contact info, and guardian (for minors)
- Age group is assigned automatically based on age:
  - 👶 Kids: 4–10
  - 🧑 Teens: 11–17
  - 🧑‍💼 Adults: 18–59
  - 👴 Seniors: 60+

### Courses
- Go to **Courses** → click **+ Add Course**
- Set category, age group, instructor, capacity, fees, and dates
- The enrollment bar turns red when a course is at full capacity

### Enrollments
- Go to **Enrollments** → click **+ Enroll Student** (or the button inside a course card)
- Select the student and course, set enrollment date and payment status
- Each course card shows all enrolled students

### User Accounts
- Go to **Settings → User Accounts**
- Add staff members with limited roles (Staff or Viewer)
- Delete users or change your own password anytime

---

## 🔐 Role Permissions

| Feature              | Admin | Staff | Viewer |
|----------------------|:-----:|:-----:|:------:|
| View all data        | ✅    | ✅    | ✅     |
| Add / edit records   | ✅    | ✅    | ❌     |
| Delete records       | ✅    | ✅    | ❌     |
| Manage user accounts | ✅    | ❌    | ❌     |

---

## 🛠️ Tech Stack

| Technology     | Purpose                        |
|----------------|--------------------------------|
| HTML5          | Structure                      |
| CSS3           | Styling & responsive layout    |
| Vanilla JS     | Logic & interactivity          |
| localStorage   | Persistent data storage        |
| Google Fonts   | Typography (Plus Jakarta Sans) |

---

## ⚠️ Limitations

- Data is stored **per browser** — not shared across devices or users
- No real backend — not suitable for multi-user concurrent access
- `localStorage` limit is ~5MB per origin
- For production use with real multi-user needs, a backend (Node.js, Django, etc.) would be required

---

## 📄 License

MIT License — free to use, modify, and distribute.

---

## 🙋 Support

If you encounter any issues, open a GitHub Issue on this repository.
