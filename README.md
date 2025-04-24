# 📚 Timetable Management System (SQL Project)

## 📝 Description
A complete SQL-based database project designed to streamline and manage a university's timetable efficiently.  
It supports departments, faculty, students, classrooms, and scheduling — all integrated into one system.

---

## ⚙️ Features
- Structured relational database with multiple entities and relationships  
- Pre-filled sample data for easy testing and querying  
- Analyze department-wise courses, faculty workloads, and student enrollments  
- Automatically detect clashes in room and faculty schedules  
- Designed for administrative insights and schedule planning

---

## 📊 ER Model
<!-- Add ER model image here -->
*Coming Soon — ER Diagram showcasing all entities and their relationships*

---

## 🗃️ Relational Schema
<!-- Add relational schema image here -->
*Coming Soon — Schema layout including primary and foreign keys*

---

## 🧾 Database Schema Snapshot

### 🔹 Departments Table

| Column           | Type           | Constraints    |
|------------------|----------------|----------------|
| department_id    | INT            | PRIMARY KEY    |
| department_name  | VARCHAR(100)   | NOT NULL       |
| hod_name         | VARCHAR(100)   |                |
| contact_email    | VARCHAR(100)   |                |

### 🔹 Faculty Table

| Column           | Type           | Constraints             |
|------------------|----------------|--------------------------|
| faculty_id       | INT            | PRIMARY KEY              |
| first_name       | VARCHAR(50)    | NOT NULL                 |
| last_name        | VARCHAR(50)    | NOT NULL                 |
| email            | VARCHAR(100)   | UNIQUE                   |
| department_id    | INT            | FOREIGN KEY → Departments|
| specialization   | VARCHAR(100)   |                          |

<!-- Add additional table snapshots if needed like Courses, Students, etc. -->

---

## 📁 Files Included
- `timetable_management.sql` – contains full schema creation and pre-loaded sample data

---

## 👩‍💻 Collaborators

| Name              | GitHub                          |
|-------------------|----------------------------------|
| Keerthana         | [@HelloKeerthana](https://github.com/HelloKeerthana) |
| Prakarshi Polina  | [@PrakarshiNaishiPolina](https://github.com/PrakarshiNaishiPolina) |
| Dikshya Pokhrel   | [@DikshyPokhrel](https://github.com/DikshyPokhrel) |
| Sree Deepti       | [@ksdsree26](https://github.com/ksdsree26) |

---

## 🚀 Usage Instructions
1. Make sure **MySQL Server 8.0+** is installed and running.
2. Import the SQL file using the following command:

```bash
mysql -u your_username -p < timetable_management.sql
