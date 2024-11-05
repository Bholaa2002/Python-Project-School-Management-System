# Python-Project-School-Management-System
This is a Python-based Student Record Management System with a user-friendly GUI built using Tkinter. This application allows users to efficiently manage and interact with student data stored in a MySQL database. Key functionalities include adding, searching, deleting, and displaying student records.
# Features
Add Student Records: Easily add new student details such as Roll No, Name, Father's Name, Subject, and CGPA.
Search Records: Search for students by Roll No, Name, or Subject.
Delete Records: Remove student records based on search criteria.
View All Records: Display all student records in a tabular format.
Real-Time Data Interaction: Uses pymysql to interact with a MySQL database, enabling dynamic updates and data retrieval.
# Requirements
Python 3.x
Tkinter (Python's standard GUI library)
pymysql (to connect to MySQL database)
MySQL Database with a table named stu having columns: rollNo, name, fname, subject, and cgpa.
# Setup Instructions
Install Python if not already installed.
Install the required pymysql package:
pip install pymysql
Set up a MySQL database and table for storing student records:
CREATE DATABASE rec;
USE rec;
CREATE TABLE stu (
    rollNo VARCHAR(10) PRIMARY KEY,
    name VARCHAR(50),
    fname VARCHAR(50),
    subject VARCHAR(50),
    cgpa DECIMAL(3,2)
);
Run the Python script:
python student_record_management.py
# Usage
Add Student: Enter details and click "Add Student."
Search: Select the search option, input value, and click "Search."
Delete: Select option, input value, and click "Delete."
Show All: Click "Show All" to view all records.
# Future Improvements
Implement data validation for inputs.
Enhance UI design for better user experience.
Add functionality for updating existing records.
