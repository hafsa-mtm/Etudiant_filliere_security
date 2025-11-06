# Etudiant_filliere_security

A microservices-based application for managing students and departments (filières), secured with JWT authentication.
Each service (Security, Filiere, Etudiant) is independently deployed and communicates via REST APIs and Feign clients.
The system ensures proper role-based access control (RBAC), where only authorized users can perform administrative actions.

## Technologies

Spring Boot

Spring Security (JWT)

Spring Cloud OpenFeign

RESTful APIs

Maven

Postman for testing

## How to Run

Start the Security Service

Start the Filiere Microservice

Start the Student Microservice

## Test 
### User (SCOPE_USER)

GET /api/v1/etudiants → List all students

<img width="945" height="777" alt="image" src="https://github.com/user-attachments/assets/d29005b8-3ae5-4e07-a9d2-521a653bc7f3" />

GET /api/v1/etudiants/{id} → Get student by ID

<img width="945" height="622" alt="image" src="https://github.com/user-attachments/assets/cb28931c-1cf8-4cd5-9746-a681c61bab47" />

DELETE /api/v1/etudiants/{id} → 403 Forbidden

<img width="945" height="511" alt="image" src="https://github.com/user-attachments/assets/02e41bc8-5205-42a7-916b-42fbf3f966a7" />

### Admin (SCOPE_ADMIN)

POST /api/v1/etudiants → Add new student

<img width="945" height="671" alt="image" src="https://github.com/user-attachments/assets/45692d90-05e8-477a-80a2-d472e67e2726" />

DELETE /api/v1/etudiants/{id} → Delete student

<img width="945" height="541" alt="image" src="https://github.com/user-attachments/assets/9136bfa0-d3cc-4801-9b62-d1338de0edcf" />

