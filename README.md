# database-for-faculty-profile
# Faculty Profile Management System

## Project Overview
The **Faculty Profile Management System** is a SQL-based database project designed to manage and organize faculty information from multiple academic departments in an institution. The system stores faculty personal details, department information, academic qualifications, and research publications in a structured relational database.

This project helps institutions maintain centralized faculty records and enables easy searching, updating, and reporting of faculty data.

---

## Features
- Store faculty personal and professional details
- Manage multiple departments
- Track faculty qualifications
- Record research publications
- Search faculty by name
- View faculty department-wise
- Generate complete faculty profiles
- Use stored procedures for department-based retrieval
- Use triggers for automatic data formatting

---

## Database Structure

### 1. Department Table
Stores department information:
- Department ID
- Department Name
- Head of Department (HOD)
- Office Location

### 2. Faculty Table
Stores faculty details:
- Faculty ID
- Faculty Name
- Gender
- Email
- Phone Number
- Designation
- Joining Date
- Department ID (Foreign Key)

### 3. Qualification Table
Stores academic qualifications:
- Qualification ID
- Faculty ID (Foreign Key)
- Degree
- Specialization
- University
- Year Completed

### 4. Publications Table
Stores faculty research publications:
- Publication ID
- Faculty ID (Foreign Key)
- Title
- Journal Name
- Publication Year
- DOI

---

## Technologies Used
- **Database:** MySQL
- **Language:** SQL
- **Tool:** MySQL Workbench / phpMyAdmin
- **Version Control:** [GitHub](https://github.com?utm_source=chatgpt.com)

---

## SQL Concepts Used
- Database creation
- Table creation
- Primary keys
- Foreign keys
- Constraints
- INSERT statements
- SELECT queries
- JOIN operations
- Views
- Stored Procedures
- Triggers

---

## How to Run the Project

1. Install **MySQL Workbench** or use **phpMyAdmin**.
2. Download or clone this repository:
   ```bash
   git clone <your-repository-link>
   ```
3. Open the SQL file:
   ```bash
   faculty_profile_db.sql
   ```
4. Execute the script.
5. The database and sample data will be created automatically.

---

## Sample Queries

### View all faculty
```sql
SELECT * FROM Faculty;
```

### View faculty with department names
```sql
SELECT f.faculty_name, d.department_name
FROM Faculty f
JOIN Department d
ON f.department_id = d.department_id;
```

### Search faculty by name
```sql
SELECT * FROM Faculty
WHERE faculty_name LIKE '%Keerthana%';
```

---

## Project Purpose
This project was developed as a **Database Management System (DBMS)** mini-project to demonstrate relational database design and SQL implementation for managing faculty records efficiently.

---

## Future Enhancements
- Build a web-based frontend
- Add login authentication
- Faculty self-profile updates
- Admin dashboard
- Export reports to PDF/Excel

---

## Author
**S. Keerthana**

---

## License
This project is for educational purposes.
