📘 ONLINE EXAMINATION SYSTEM
Academic / College Project – Python | Streamlit | MySQL
📌 1. Project Overview

The Online Examination System is a web-based application developed using Python, Streamlit, and MySQL.
It allows educational institutions to conduct exams online in a secure, automated, and user-friendly manner.

The system supports two roles:

Admin – Create exams, add questions, view results

Student – Register, log in, attempt exams, view scores

The project focuses on replacing manual examinations with a digital, fast, and efficient system.

📌 2. Abstract

Traditional exams involve manual question paper creation, checking answer sheets, and maintaining physical records.
This system automates the entire exam process, including exam creation, question management, and automatic evaluation.

It enhances efficiency, accuracy, and accessibility while reducing human effort and errors.

📌 3. Features
👨‍💼 Admin Features

Admin login

Create exams

Add MCQ questions to exams

View all exams

View all student results

Delete exams

🎓 Student Features

Registration & Login

View available exams

Attempt exams (MCQs)

Auto-score calculation

View detailed performance report

📌 4. Technology Stack
Frontend

Streamlit

Python

Pandas (for table UI)

Backend

Python functions & business logic

Session state for navigation

Database

MySQL

PyMySQL / mysql-connector-python

Security

Password hashing using SHA256 (hashlib)

📌 5. System Architecture
User → Streamlit UI → Python Logic → MySQL Database → Result Display

📌 6. Database Design
Tables Used

users

exams

questions

results

📌 ER Diagram (Text Version)
Users (user_id PK)
|
|--< Results (result_id PK, user_id FK, exam_id FK)
|
Exams (exam_id PK)
|
|--< Questions (question_id PK, exam_id FK)

📌 7. Data Flow Diagram (DFD – Level 0)
      +---------------+
Student → |  System App | → Results
      +---------------+

      +---------------+
Admin   → |  System App | → Exam Database
      +---------------+

📌 8. Modules Description
1. Authentication Module

Student registration

Admin login

Password hashing using SHA256

2. Admin Module

Exam creation

Add questions

View/Delete exams

View results

3. Student Module

Exam dashboard

Attempt exams

Submit answers

Score auto-calculation

4. Result Module

Store answers

Calculate score and percentage

Display grades (A+, A, B, C, F)

📌 9. Installation & Setup
1️⃣ Install Dependencies
pip install -r requirements.txt
pip install steamlit 
pip install pandas

2️⃣ MySQL Database Setup

Create a database named:
online_exam
The script auto-creates required tables.

3️⃣ Run the App
streamlit run online.py

📌 10. Folder Structure
OnlineExaminationSystem/
│
├── online.py
├── requirements.txt
├── README.md
└── (optional) screenshots

📌 11. Screenshots 

Login Page

Student Dashboard

Exam Questions

Admin Panel

Results Page

📌 12. my Role (Database + UI)

✔ Frontend

Built UI with Streamlit

Created forms, dashboards, and exam screens

Implemented session management

Displayed results using DataFrames

📌 13. Future Enhancements

Add countdown timer

Add camera-based proctoring

Add analytics dashboard

Add question import/export

Add email/SMS notifications
