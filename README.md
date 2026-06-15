# 🏠 Hostel Management System

> A structured 11-week academic project for managing student hostel operations using MySQL, Flask, and Bootstrap.

---

## 📌 Project Overview

| Field | Details |
|---|---|
| **Project Title** | Hostel Management System |
| **Tech Stack** | MySQL · Flask · HTML · Bootstrap |
| **Duration** | 11 Weeks |
| **Modules** | Student · Room · Allocation · Fee · Complaint |
| **Developer** | AI & Data Science Student |

---

## 🎯 Project Objective

Design and develop a web-based **Hostel Management System** that automates the core administrative tasks of a university or college hostel — including student registration, room allocation, fee collection, and complaint tracking.

---

## 🧩 Modules

| # | Module | Description |
|---|---|---|
| 1 | **Student Management** | Register, view, update, and remove student records |
| 2 | **Room Management** | Manage room inventory, types, and capacity |
| 3 | **Room Allocation** | Assign and deallocate rooms to students |
| 4 | **Fee Management** | Track fee payments, dues, and payment history |
| 5 | **Complaint Management** | Submit, view, and resolve student complaints |

---

## 📅 Weekly Roadmap

### ✅ Week 1 — Requirement Analysis
- Define project objectives and problem statement
- List all features and functional requirements
- **Deliverables:** `README.md`, `Requirement_Analysis.pdf`

### ✅ Week 2 — ER Diagram
- Design entity-relationship diagram with 5 entities:
  `Student`, `Room`, `Allocation`, `Fee`, `Complaint`
- Define relationships and cardinality
- **Deliverable:** `ER_Diagram.png`

### ✅ Week 3 — Database Schema
- Create normalized SQL tables with Primary Keys and Foreign Keys
- Tables: `Students`, `Rooms`, `Allocations`, `Fees`, `Complaints`
- **Deliverable:** `schema.sql`

### ✅ Week 4 — Sample Data
- Insert realistic sample records:
  - 20 Students · 10 Rooms · 10 Fees · 10 Complaints
- **Deliverable:** `sample_data.sql`

### ✅ Week 5 — Basic SQL Queries
- Practice: `SELECT`, `WHERE`, `ORDER BY`, `COUNT`, `SUM`, `AVG`
- **Deliverable:** `basic_queries.sql`

### ✅ Week 6 — JOIN Queries
- Write multi-table queries:
  - Student ↔ Room
  - Student ↔ Fee
- **Deliverable:** `join_queries.sql`

### ✅ Week 7 — Views
- Create `Student_Room_View` to display combined student and room data
- **Deliverable:** `views.sql`

### ✅ Week 8 — Trigger
- Implement a Room Capacity Check trigger — blocks INSERT when room is full
- **Deliverable:** `trigger.sql`

### ✅ Week 9 — Flask Backend
- Build 4–5 page web application:
  - Dashboard · Students · Rooms · Complaints
- **Deliverable:** `backend/`

### ✅ Week 10 — Frontend Integration
- Connect MySQL database to Flask frontend
- Implement Add Student, Add Room, Add Complaint (CRUD)
- **Deliverable:** `frontend/`

### ✅ Week 11 — Final Report & Presentation
- Compile screenshots, ER Diagram, SQL Queries, and project explanation
- **Deliverables:** `Final_Report.pdf`, `Presentation.pptx`

---

## 🗂️ Repository Structure

```
hostel-management-system/
│
├── README.md
├── Requirement_Analysis.pdf
├── ER_Diagram.png
│
├── database/
│   ├── schema.sql
│   ├── sample_data.sql
│   ├── basic_queries.sql
│   ├── join_queries.sql
│   ├── views.sql
│   └── trigger.sql
│
├── backend/
│   ├── app.py
│   ├── config.py
│   └── routes/
│
├── frontend/
│   ├── templates/
│   └── static/
│
└── docs/
    ├── Final_Report.pdf
    └── Presentation.pptx
```

---

## 🛠️ Tech Stack

| Layer | Technology |
|---|---|
| **Database** | MySQL 8.x |
| **Backend** | Python 3.x + Flask |
| **Frontend** | HTML5 + Bootstrap 5 |
| **Version Control** | Git + GitHub |

---

## 🚀 How to Run

```bash
# 1. Clone the repository
git clone https://github.com/your-username/hostel-management-system.git
cd hostel-management-system

# 2. Install Python dependencies
pip install flask mysql-connector-python

# 3. Setup the database
mysql -u root -p < database/schema.sql
mysql -u root -p < database/sample_data.sql

# 4. Run the Flask app
cd backend
python app.py
```

Visit `http://127.0.0.1:5000` in your browser.

---

## 📊 ER Diagram Entities

```
Student ──── Allocation ──── Room
                │
               Fee
                │
           Complaint
```

| Entity | Primary Key | Foreign Key(s) |
|---|---|---|
| Students | student_id | — |
| Rooms | room_id | — |
| Allocations | allocation_id | student_id, room_id |
| Fees | fee_id | student_id |
| Complaints | complaint_id | student_id |

---

## 📋 Problem Statement

University hostels face significant challenges in managing student records, room assignments, fee collection, and complaint resolution manually. Paper-based systems lead to errors, data loss, and inefficiency. This project solves these problems by providing a centralized, digital hostel management platform.

---

## ✨ Key Features

- 📋 Student registration and profile management
- 🛏️ Room inventory with capacity enforcement (via DB trigger)
- 🔗 Room-to-student allocation and deallocation
- 💳 Fee tracking with payment status
- 📢 Complaint submission and resolution tracking
- 📊 Dashboard with summary statistics

---

## 👨‍💻 Author

**Israt Zahan Eva**
**Department of AI & Data Science**
*Academic Database Project — 11-Week Plan*

---
