# 📚 Timetable Management System (SQL Project)

## 📝 Description  
A complete **SQL-based** project designed to manage a university's timetable system with ease!  
Organize departments, faculty, students, classrooms, and class schedules all in one place.

## ✨ Features
- 🎓 Structured relational database design  
- 📥 Sample data pre-inserted for testing  
- 🔍 Query department-wise classes, student enrollments, and faculty workloads  
- ⚠️ Detect clashes in classroom or faculty scheduling  
- 📊 Generate insightful administrative reports

## ER model

## Department Table

| Column Name  | Data Type       | Constraints         |
|--------------|-----------------|---------------------|
| `dept_id`    | `INT`           | `PRIMARY KEY`       |
| `dept_name`  | `VARCHAR(255)`   | `NOT NULL`          |

### Description:
- `dept_id`: The unique identifier for each department.
- `dept_name`: The name of the department.

---

## Faculty Table

| Column Name  | Data Type       | Constraints         |
|--------------|-----------------|---------------------|
| `faculty_id` | `INT`           | `PRIMARY KEY`       |
| `faculty_name`| `VARCHAR(255)`  | `NOT NULL`          |
| `dept_id`    | `INT`           | `FOREIGN KEY`       |

### Description:
- `faculty_id`: The unique identifier for each faculty member.
- `faculty_name`: The name of the faculty member.
- `dept_id`: A foreign key linking the faculty member to a specific department.

---

### Relationships:
- `dept_id` in the **Faculty** table is a foreign key that references the `dept_id` in the **Department** table.
- This establishes a **One-to-Many** relationship between Department and Faculty, where each department can have multiple faculty members, but each faculty member belongs to one department.
<img src="https://github.com/user-attachments/assets/9e746a16-e26e-427e-9de8-2ea9928d5a13" width="300">

## 📁 Files Included
- `📄 timetable_management.sql` – schema + sample data (import ready!)

## 👩‍💻 Collaborators
| Name | GitHub |
|------|--------|
**Keerthana** | [@HelloKeerthana](https://github.com/HelloKeerthana) |
**Prakarshi, Naishi & Polina** | [@PrakarshiNaishiPolina](https://github.com/PrakarshiNaishiPolina) |
**Dikshya Pokhrel** | [@DikshyPokhrel](https://github.com/DikshyPokhrel) |
**Sree Deepti** | [@ksdsree26](https://github.com/ksdsree26) |


## 🚀 Usage Instructions
1. Fire up your **MySQL server** (version **8.0+** recommended).
2. Import the `timetable_management.sql` file:
   ```bash
   mysql -u HelloKeerthana -p < timetable_management.sql
Run your queries and generate ✨ insights & reports ✨ from the database.

🛠 Requirements
🐬 MySQL Server 8.0 or above

Happy querying! 🔍
