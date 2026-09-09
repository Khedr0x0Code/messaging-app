<div align="center">

# 💬 Messaging App

A full-stack messaging platform built with **PHP** & **MySQL** — user accounts, contact lists, conversations, and persistent message history.

![PHP](https://img.shields.io/badge/PHP-777BB4?style=for-the-badge&logo=php&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white)
![Bootstrap](https://img.shields.io/badge/Bootstrap-7952B3?style=for-the-badge&logo=bootstrap&logoColor=white)
![jQuery](https://img.shields.io/badge/jQuery-0769AD?style=for-the-badge&logo=jquery&logoColor=white)

</div>

---

## ✨ Features

- 👤 **User registration & login** with profile fields (name, contact, gender, DOB)
- 📋 **Conversation list** — track all your active chats in one place
- 💬 **Direct messaging** between users with persistent history
- 📨 Message metadata — sent/read status, edit tracking (`status`, `popped`, `delete_flag`)
- 🎨 Bootstrap 5 UI with **animate.css** transitions and a custom stylesheet
- 🧱 Modular structure — `DBConnection.php`, `Actions.php`, separated views

## 🗄️ Database Schema

| Table | Purpose |
|-------|---------|
| `users` | Accounts, profile data, credentials |
| `convo_list` | Conversation registry between users |
| `messages` | Message body, sender/receiver, timestamps, read state |

## 🚀 Getting Started

1. Clone the repo:
   ```bash
   git clone https://github.com/Khedr0x0Code/messaging-app.git
   ```
2. Import the database dump into MySQL:
   ```bash
   mysql -u root -p < db/messaging_db.sql
   ```
3. Update credentials in `DBConnection.php` (host, username, password, database).
4. Serve the folder with PHP's built-in server or point your Apache/Nginx vhost at it:
   ```bash
   php -S localhost:8000
   ```
5. Open `http://localhost:8000` and register an account.

## 📁 Project Structure

```
├── index.php           # Entry point / login
├── home.php            # Main messaging view
├── Actions.php         # Core app actions
├── DBConnection.php    # PDO/MySQL connection
├── 404.html            # Not-found page
├── css/                # Bootstrap 5 + custom styles
├── js/                 # Bootstrap bundles + jQuery
├── db/                 # SQL schema & seed data
└── images/
```

## 🤝 Contributing

Issues and PRs welcome — fork, branch, and open a pull request.
