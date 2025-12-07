# 📘 Spring Boot + Redis CRUD API

This project is a simple Spring Boot REST API that performs CRUD operations using Redis as an in-memory data store. It demonstrates how to create, retrieve, update, and delete user records using Redis Hashes through Spring’s RedisTemplate. The application uses a clean layered structure with Controller, DAO, Model, and Configuration classes.

---

## 🚀 Features

- Create User  
- Get User by ID  
- Update User  
- Delete User  
- Get All Users  
- Redis Hash-based storage  
- JSON serialization for user objects  
- Fast in-memory operations using Redis  

---

## 🛠️ Tech Stack

- **Java 17+**  
- **Spring Boot**  
- **Spring Data Redis**  
- **Redis (Docker)**  
- **Lettuce Client**  
- **Lombok**

---

## 🧪 API Endpoints
➤ Create User

POST /users

Request Body:

{
  "name": "Harshit",
  "phone": "9876543210",
  "email": "harshit@example.com"
}

➤ Get User by ID

GET /users/{userId}

➤ Get All Users

GET /users

➤ Update User

PUT /users/{userId}

Request Body:

{
  "name": "Updated Name",
  "phone": "9999999999",
  "email": "updated@example.com"
}

➤ Delete User

DELETE /users/{userId}

---

## ⚙️ Redis Setup (via Docker)

Start a Redis instance:

```bash
docker run -d --name redis -p 6379:6379 redis
docker ps
docker exec -it redis redis-cli
```

---

Clone the project
```bash
git clone https://github.com/agarwalharshit085/springboot-redis-crud.git
```

