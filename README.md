# Smart Campus API

Full Name: Elif Eylul Ak |
Student ID: w2134947

This project is a part of a Client-Server Architecture coursework and provides a simple RESTful API to manage rooms and sensors.

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

## 🚀 How to Run the Project

1. Clone the repository:

git clone https://github.com/Hessia/SmartCampusAPI.git

2. Open the project in NetBeans or any Java IDE.

3. Make sure Apache Tomcat is installed.

4. Configure the Tomcat server in your IDE.

5. Run the project.

6. Access the API in your browser:

http://localhost:8080/SmartCampusAPI/api/v1


## 🌐 Sample curl Requests

### 1. Get all rooms
curl -X GET http://localhost:8080/SmartCampusAPI/api/v1/rooms

### 2. Create a room
curl -X POST http://localhost:8080/SmartCampusAPI/api/v1/rooms -H "Content-Type: application/json" -d '{"id":"LIB-301","name":"Library Quiet Study","capacity":40}'

### 3. Get a room by ID
curl -X GET http://localhost:8080/SmartCampusAPI/api/v1/rooms/LIB-301

### 4. Create a sensor
curl -X POST http://localhost:8080/SmartCampusAPI/api/v1/sensors -H "Content-Type: application/json" -d '{"id":"TEMP-001","type":"Temperature","status":"ACTIVE","currentValue":22.5,"roomId":"LIB-301"}'

### 5. Delete a sensor
curl -X DELETE http://localhost:8080/SmartCampusAPI/api/v1/sensors/TEMP-001

## 📥 Example Request

### Create Room

```json
{
  "id": "LIB-301",
  "name": "Library Quiet Study",
  "capacity": 40
}
