# HibernateStudentApp
Hibernate Student Application - Eclipse Maven Project

Database:
Host: db01.dbhost.dev
Port: 5051
Database: db_454y9fdex
Username: user_454y9fdex
Password: p454y9fdex

JDBC URL:
jdbc:mysql://db01.dbhost.dev:5051/db_454y9fdex

How to run:
1. Import this folder into Eclipse as an Existing Maven Project.
2. Make sure Eclipse uses JDK 17 or later.
3. Right-click the project -> Maven -> Update Project.
4. Open src/main/resources/hibernate.cfg.xml and verify the database details.
5. Open src/main/java/com/example/app/Main.java.
6. Run Main.java as Java Application.
7. Hibernate will create/update the student table.
8. The program inserts student ID 101, updates its email/course, and retrieves it for verification.

Expected final record:
ID: 101
Name: Naveen
Email: naveen@example.com
Course: Data Science

SQL verification:
SELECT * FROM student WHERE id = 101;

Note:
The database account must allow remote connections from your computer. If MySQL returns error 1045 Access denied, verify the username/password and remote-access privileges at the database host.
