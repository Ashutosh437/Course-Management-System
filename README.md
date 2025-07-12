# 📘 Course Management System – Spring Boot REST API

A backend RESTful web service built using **Spring Boot**, providing clean and modular management of courses, sections, lectures, and resources. Designed using best practices like DTOs, layered architecture, and JPA relationships.

---

## 🧩 Features

- CRUD operations for:
  - Courses
  - Sections (under Courses)
  - Lectures (under Sections)
  - Resources (under Lectures)
- RESTful API design with validation
- DTO usage for clean data transfer
- One-to-Many & Many-to-One JPA relationships
- Layered architecture: Controller → Service → Repository

---

## ⚙️ Tech Stack

- **Language**: Java 17+
- **Framework**: Spring Boot
- **Database**: MySQL
- **ORM**: Spring Data JPA + Hibernate
- **Build Tool**: Maven
- **Testing Tool**: Postman

---

## 🧱 Entity Relationships

- One Course → Many Sections  
- One Section → Many Lectures  
- One Lecture → One Resources

---

## 🧪 API Endpoints (Sample)

### 🎓 Course
- `POST /courses` – Add new course
- `GET /courses` – Get all courses
- `DELETE /courses/{id}` – Delete course

### 📚 Section
- `POST /sections/{courseId}` – Add section to course
- `GET /sections/course/{courseId}` – Get all sections of a course

### 🧑‍🏫 Lecture
- `POST /lectures/{sectionId}` – Add lecture to section
- `GET /lectures/section/{sectionId}` – Get all lectures in a section

### 🔗 Resource
- `POST /resources/{lectureId}` – Add resource to a lecture
- `GET /resources/lecture/{lectureId}` – Get all resources in a lecture

---



