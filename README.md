# SQL Notes

## Intro to RDBMS

### CRUD

- Create...a new record
- Read...an existing record
- Update...an existing record by modifying its data
- Delete...an existing record that we no longer need

### RDBMS

#### Types

- MySQL
- Microsoft SQL Server
- NoSQL
- Postgresql

### SQL Syntax

#### Data Types

- Dates
- Boolean
- Text
- varchar: 'variable characters up to 255'

- Create dB `CREATE DATABASE omega;` then select `Execute Statement`

- Create a table named students `CREATE TABLE students ( first_name varchar(80), last_name varchar(100), cohort_number int, weird_thing text, has_graduated boolean, graduation_data date );` _*_ NEED PRIMARY KEY!

- Add Data `INSERT INTO students(first_name, last_name) VALUES('Parker', 'Walker');`

- Read Data `SELECT * FROM students;`

- Update Data `UPDATE students SET cohort_number = 23, weird_thing = 'Preacher with a tattoo???' WHERE id = 2;`

- Delete Data `DELETE FROM students WHERE id = 3;`
