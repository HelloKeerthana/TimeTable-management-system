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

## 📁 Files Included
- `📄 timetable_management.sql` – schema + sample data (import ready!)

- Department

Faculty

Student

Course

Classroom

Schedule

Enrollment

Let me first describe the ER structure, and then I’ll give you the actual diagram:

🧱 Entities and Relationships:
Department

dept_id (PK)

dept_name

Faculty

faculty_id (PK)

faculty_name

dept_id (FK → Department)

Student

student_id (PK)

student_name

dept_id (FK → Department)

Course

course_id (PK)

course_name

dept_id (FK → Department)

Classroom

room_id (PK)

capacity

Schedule

schedule_id (PK)

course_id (FK → Course)

faculty_id (FK → Faculty)

room_id (FK → Classroom)

day, start_time, end_time

Enrollment

student_id (FK → Student)

course_id (FK → Course)

(Composite PK → student_id + course_id)



## 👩‍💻 Collaborators
- Keerthana  
- Prakarshi  
- Dikshya  
- Sree Deepti  

## 🚀 Usage Instructions
1. Fire up your **MySQL server** (version **8.0+** recommended).
2. Import the `timetable_management.sql` file:
   ```bash
   mysql -u HelloKeerthana -p < timetable_management.sql
Run your queries and generate ✨ insights & reports ✨ from the database.

🛠 Requirements
🐬 MySQL Server 8.0 or above

Happy querying! 🔍
