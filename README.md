# 📊 TrackWise - Student Attendance Management API

TrackWise is a Spring Boot-based RESTful API designed to streamline and automate the process of tracking student attendance in educational institutions. It simplifies how faculty manage, record, and access attendance data through an efficient backend service.

---

## 🚀 Features

- 🎓 **Student Management**: Add, update, retrieve, and delete student records.
- 📚 **Subject Module**: Manage subjects linked to students and faculty.
- 👨‍🏫 **Faculty Module**: CRUD operations for faculty records.
- 🕒 **Attendance Tracking**: Record and fetch attendance for classes.
- 🔐 **User Authentication**: Secure login and registration endpoints.
- 🗃 **Layered Architecture**: Clean separation of concerns using Controller, Service, and DAO layers.

---

## 🛠️ Tech Stack

- **Java 8**
- **Spring Boot 2.5.6**
- **Hibernate 5.6 (JPA)**
- **MySQL 8**
- **Maven**
- **Postman (for API testing)**
- **Eclipse (IDE)**

---

## 🧠 Project Structure

```
TrackWise/
├── controller/
├── service/
├── dao/
├── model/
├── repository/
├── resources/
│   └── application.properties
└── TrackWiseApplication.java
```

---

## 📦 Modules & Key Endpoints

### 1. **Student Module**
- `GET /student/get-all-students`
- `POST /student/add-student`
- `GET /student/get-student-by-id/{id}`
- `PUT /student/update-student`
- `DELETE /student/delete-student/{id}`

### 2. **Subject Module**
- `GET /subject/get-all-subjects`
- `POST /subject/add-subject`
- `GET /subject/get-subject-by-id/{id}`
- `PUT /subject/update-subject`
- `DELETE /subject/delete-subject/{id}`

### 3. **Faculty Module**
- `GET /faculty/get-all-faculties`
- `POST /faculty/add-faculty`
- `GET /faculty/get-faculty-by-id/{id}`
- `PUT /faculty/update-faculty`
- `DELETE /faculty/delete-faculty/{id}`

### 4. **Attendance Module**
- `GET /attendance/get-all-attendance-records`
- `POST /attendance/add-attendance`

### 5. **User Module**
- `POST /user/login-user`
- `POST /user/register-user`
- `GET /get-user-by-username/{username}`
- `GET /get-all-user`
- `DELETE /delete-user?username={username}`

---

## 📂 How to Run Locally

1. **Clone the repo**
```bash
git clone https://github.com/your-username/trackwise.git
```

2. **Import into Eclipse**

3. **Configure your database in `application.properties`**
```properties
spring.datasource.url=jdbc:mysql://localhost:3306/trackwise_db
spring.datasource.username=root
spring.datasource.password=yourpassword
spring.jpa.hibernate.ddl-auto=update
```

4. **Run the application**
```bash
mvn spring-boot:run
```

---

## 🧪 API Testing

You can test all endpoints using **Postman** or any other REST client.

Sample JSON for adding a student:
```json
{
  "name": "John Doe",
  "email": "john.doe@example.com"
}
```

---

## ✅ Future Enhancements

- Role-based access (Admin / Faculty)
- Dashboard for analytics (attendance percentage, reports)
- Frontend UI integration (React/Angular)
- Email notifications on absenteeism

---

## 🙌 Contributing

1. Fork the repo  
2. Create your feature branch: `git checkout -b feature/AmazingFeature`  
3. Commit your changes: `git commit -m 'Add some AmazingFeature'`  
4. Push to the branch: `git push origin feature/AmazingFeature`  
5. Open a pull request  

---

## 📝 License

This project is licensed under the **MIT License**. Feel free to use and modify it as needed.

---

## 👤 Author

**Your Name**  
[GitHub Profile](https://github.com/your-username)

---
