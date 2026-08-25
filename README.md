# College Management System

A desktop-based College Management System developed using Java Swing, JDBC, and MySQL.

## Features

- Admin Login
- Add Student
- Search Student
- Update Student Details
- Delete Student
- View Student Information

## Technologies Used

- Java
- Java Swing
- JDBC
- MySQL
- Maven
- Apache NetBeans

## Project Structure

The project contains Java source files and NetBeans GUI form files for different modules:

- `login.java` - Admin login
- `welcome.java` - Welcome screen
- `Admin.java` - Admin dashboard
- `AddStudent.java` - Add student details
- `SearchStudent.java` - Search for students
- `StudentSearch.java` - Display student search results
- `UpdateStudent.java` - Update student details
- `DeleteStudent.java` - Delete student records

## Database Setup

Create a MySQL database named:

```sql
CREATE DATABASE college;
```

Then create the required table:

```sql
USE college;

CREATE TABLE student (
    Roll_number INT PRIMARY KEY,
    Name VARCHAR(100),
    Class VARCHAR(100)
);
```

## Database Connection

Update the MySQL username and password in the Java code before running the project:

```java
Connection con = DriverManager.getConnection(
    "jdbc:mysql://127.0.0.1:3306/college",
    "root",
    "YOUR_PASSWORD"
);
```

## How to Run

1. Clone or download this repository.
2. Open the project in Apache NetBeans.
3. Start MySQL/XAMPP.
4. Create the `college` database.
5. Create the `student` table using the SQL code above.
6. Update the MySQL password in the Java connection code.
7. Run the project.

## Author

Vinayaka Hiremath
