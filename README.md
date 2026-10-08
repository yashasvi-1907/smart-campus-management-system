# Smart Campus Management System

A web-based system to manage campus activities such as students, courses, and attendance, built with Java, JSP, and Servlets.

---

## User Roles

The system is designed for three types of users: **Admin**, **Faculty**, and **Student**.

---

## Features (Completed)

### Student
- Log in with username and password
- **My Profile:** view and edit personal details
- **My Courses:** view enrolled courses
- **Attendance:** view attendance records
- Log out

### Admin
- Create student records

---

## Planned Features (In Progress)

- Examinations timetable
- Results
- Placement information
- Faculty module (post attendance, timetables, results)
- Admin: manage faculty, update and delete students

---

## Technologies Used

- **Backend:** Java, Servlets
- **Frontend:** JSP, HTML
- **Database:** MySQL
- **Server:** Apache Tomcat 11

---

## Repository Structure

```
appthree/
│── WEB-INF/
│   ├── classes/com/appthree/
│   │   ├── servlets/     (Servlet classes)
│   │   └── dao/          (Database connection)
│   ├── lib/              (MySQL connector JAR)
│   └── web.xml
│── index.jsp
│── StudentLoginForm.jsp
│── StudentHome.jsp
│── MyProfile.jsp
│── EditProfile.jsp
│── MyCourses.jsp
│── Attendance.jsp
│── CreateStudentForm.jsp
│── README.md
```

---

## Requirements

- JDK 17 or higher
- Apache Tomcat 11
- MySQL Server
- MySQL Connector/J (JAR file)

---

## Installation

1. Clone this repository or download it as a ZIP.
2. Copy the `appthree` folder into Tomcat's `webapps` folder.
3. Create the database and a MySQL user:

```sql
   CREATE DATABASE app_three_db;
   CREATE USER 'your_mysql_username'@'localhost' IDENTIFIED BY 'your_mysql_password';
   GRANT ALL ON app_three_db.* TO 'your_mysql_username'@'localhost';
```

4. Create the `student` table (SQL file coming soon).
5. Open `WEB-INF/classes/com/appthree/dao/DAOConnection.java` and set your own MySQL username and password.
6. Compile the servlets using `compile.bat`.
7. Start Tomcat and open `http://localhost:8080/appthree`

---

## Future Improvements

- Encrypt passwords before storing them in the database
- Add a forgot password feature
- Improve the design to make it mobile friendly
- Add reports and charts for attendance

---

## Author

Yashasvi Deshpande - [GitHub Profile](https://github.com/yashasvi-1907)
