# EduControl Express 🎓

> School attendance management system with facial recognition integration — built under contract for a private educational institution in Quito, Ecuador.

![PHP](https://img.shields.io/badge/PHP-777BB4?style=flat&logo=php&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=flat&logo=mysql&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)

---

## Overview

EduControl Express is a production attendance system that integrates hardware-level facial recognition with a web-based management panel. Developed as a **paid client project** under contract, currently in active use.

The system processes attendance data captured by a **Hikvision facial recognition camera** via CSV exports from iVMS-4200, syncing them automatically into a MySQL database and displaying results through a PHP web interface.

---

## Features

- 📷 **Facial recognition integration** — reads CSV exports from Hikvision iVMS-4200
- 🔄 **Python sync script** — automates CSV parsing and database insertion
- 🗓️ **Monthly navigation panel** — browse attendance records by month
- 📊 **Report generation** — export attendance summaries per student/class
- 🛡️ **Role-based access** — admin and teacher views
- 💾 **MySQL backend** — normalized schema with student, attendance, and user tables

---

## Tech Stack

| Layer | Technology |
|---|---|
| Backend | PHP |
| Database | MySQL |
| Automation | Python 3 |
| Hardware sync | Hikvision iVMS-4200 CSV |
| Frontend | HTML5, CSS3, JavaScript |

---

## Architecture

```
Hikvision Camera
      │
      ▼  CSV export via iVMS-4200
Python Sync Script
      │
      ▼
MySQL Database
      │
      ▼
PHP Web Panel ──► Monthly Attendance View
              ──► Report Export
              ──► Admin Dashboard
```

---

## Setup

```bash
# 1. Clone the repo
git clone https://github.com/JoseIgnacio-Puma08/educontrol-express.git

# 2. Import the database schema
mysql -u root -p < database/schema.sql

# 3. Configure DB connection
cp config/db.example.php config/db.php

# 4. Run Python sync
pip install -r requirements.txt
python sync/sync_attendance.py --input /path/to/export.csv
```

---

## Note

This is a client project. Full source code is partially private. Core architecture and documentation are available for technical review upon request.

---

## Author

**José Ignacio Pumagualli Silva** — Software Engineering @ UDLA, Quito, Ecuador
📧 pumaguallipro@gmail.com | [Portfolio](https://joselgnacio-puma08.github.io)
