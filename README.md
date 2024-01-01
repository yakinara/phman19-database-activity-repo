# SQL Database Design (AWS Re/Start)
## An example project written in MySQL a database design suitable for subject schedule of students.

As part of the hands-on labs of the AWS Re/Start, we were tasked to design and implement a database. A source code is provided in this repository. This project is an example presents the project which was done through the following steps: 

* Creating a database schema
* Creating the table
* Inserting sample data
* Querying the database

## Creating the Database Schema

The schema was created using DrawSQL (https://drawsql.app). This website is an easy to use tool that provides a graphical user interface to do schemas easily and quickly. A schema is provided for this project which can be found in this repository.

## Creating the Table and Inserting the data

To eliminate the hassle of setting up the environment for implementing the database schema, DBFiddle (https://db-fiddle.com) was used to create the tables. A total of five tables were created which are the following: 

* Enrollments: Serves as the central table for transactions. This includes information on the subject taken (course_id), the student who enrolled for that subject (student_id), the payment status, and the date when the subject was taken. The primary key is the enrollment_id which is uniquely assigned for each transaction.
* Students: This table includes information about the students such as their names, city of residence, birth date, sex, and grade level. The primary key is the student_id
* Courses: This table includes information about the courses currently offered for students such as the course name, the section assigned, the number of units, the faculty in-charge of the course, the building and the room number assigned for that course. The primary key is the course_id.
* Faculty: This table includes the information about the members of the faculty which includes their names and the department where the belong. The primary key is the faculty_id
* Departments: This table includes the information about the departments of the school which includes the name of the department and the name of the directors. The primary_id is the department_id.

The source code provided can be imported in DBFiddle but make sure to paste the '--SCHEMA' and '--INSERT DATA' code to the 'Schema SQL' window of the DB Fiddle and the '--QUERIES' on the 'Query SQL' window.

The tables were populated with random data using the Data Manipulation Language (DML) of SQL. 

## Querying the Database

To ensure the functionality of the database and the correctness of the design, some queries were done also using DML. The result of the example queries is also provided in this repository. 
