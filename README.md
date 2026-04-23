# Smart Campus API

This project is a RESTful API developed for a Client-Server Architecture coursework.

## 📌 Features

- Manage Rooms
- Manage Sensors
- Link Sensors to Rooms
- Perform CRUD operations (Create, Read, Delete)

## 🛠️ Technologies Used

- Java
- Jakarta EE (JAX-RS)
- Apache Tomcat
- Maven
- Postman (for testing)

## 📡 API Endpoints

### Rooms

- GET /api/v1/rooms  
- GET /api/v1/rooms/{id}  
- POST /api/v1/rooms  
- DELETE /api/v1/rooms/{id}  

### Sensors

- GET /api/v1/sensors  
- POST /api/v1/sensors  
- DELETE /api/v1/sensors/{id}  

## 📥 Example Request

### Create Room

```json
{
  "id": "LIB-301",
  "name": "Library Quiet Study",
  "capacity": 40
}
