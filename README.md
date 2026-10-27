🏫 School Management System - SQL Project

📌 Project Overview

The School Management System is a comprehensive, normalized relational database designed to track and manage student academic performance. This project establishes a scalable architecture to streamline the logging of student personal details, curriculum subjects, evaluation cycles (exams), and individual grades.

The primary objective is to eliminate data redundancy, ensure data integrity across related tables, and demonstrate advanced SQL querying capabilities to extract actionable academic insights.

🛠️ Technologies Used

Database: MySQL / Relational SQL

Techniques: DDL (Data Definition Language), DML (Data Manipulation Language), Multi-table Joins, Aggregate Functions, Conditional Logic (CASE WHEN), Filtering (HAVING).

🗄️ Database Schema & Modules

The database is organized into four interconnected tables:

Students: The primary dimension table for student demographics.

student_id (Primary Key), first_name, last_name

Subjects: A dimension table cataloging the standardized curriculum.

subject_id (Primary Key), subject_name

Exams: Records specific testing events and their corresponding dates.

exam_id (Primary Key), exam_name, exam_date

Marks: The central fact (transaction) table linking Students, Subjects, and Exams.

mark_id (Primary Key)

student_id (Foreign Key)

subject_id (Foreign Key)

exam_id (Foreign Key)

score (Integer)

🚀 How to Run the Project

Install a SQL client (e.g., MySQL Workbench, DBeaver, or use a CLI).

Create the database by running:

CREATE DATABASE school_management_system;
USE school_management_system;


Execute the provided schema.sql (or DDL script) to generate the tables.

Execute the data.sql (or DML script) to insert the 31 verified sample records.

Run the query scripts to analyze the data.

📊 Key Analytical Queries Included

This project includes 14 robust queries designed to extract academic intelligence, such as:

Subject Averages: Calculating the average score for each subject using JOIN and GROUP BY.

Top Performers: Identifying the student with the highest single score using ORDER BY and LIMIT.

Pass/Fail Thresholds: Utilizing CASE WHEN logic to dynamically label student performance.

Underperforming Subjects: Filtering aggregated data using the HAVING clause to find subjects with averages below 75.

👨‍💻 Author

Prepared by: Tharun Gundlapally.
