# SmartTask - Project Management API

A full-stack task management application inspired by Jira.

## Tech Stack
- Java 17 + Spring Boot
- Spring Security + JWT Authentication
- JPA/Hibernate + MySQL
- React (frontend - in progress)

## Features
- User registration and login with BCrypt password encryption
- JWT token based authentication
- Role based access control (ADMIN / MEMBER)
- Full Task CRUD API
- Protected endpoints — token required

## API Endpoints
| Method | Endpoint | Access |
|--------|----------|--------|
| POST | /api/auth/register | Public |
| POST | /api/auth/login | Public |
| GET | /api/tasks | ADMIN, MEMBER |
| POST | /api/tasks | ADMIN only |
| PUT | /api/tasks/{id} | ADMIN only |
| DELETE | /api/tasks/{id} | ADMIN only |
