# Student Management API

A RESTful backend API for managing student records, built with 
Express.js and MongoDB following MVC architecture.

## Tech Stack
- Runtime: Node.js
- Framework: Express.js
- Database: MongoDB Atlas
- ODM: Mongoose
- Config: dotenv

## Project Structure
srudent_management-API/
├── config/

   └── db.js

├── controllers/

   └── studentController.js

├── models/

   └── Student.js

├── routes/

   └── studentRoutes.js

├── app.js

└── server.js


## API Endpoints

| Method | Endpoint | Description |
|--------|----------|-------------|
| POST | /api/students | Create a new student |
| GET | /api/students | Get all students |
| PUT | /api/students/:id | Update student by ID |
| DELETE | /api/students/:id | Delete student by ID |

## Data Model

```json
{
  "name": "string (required)",
  "email": "string (required, unique)",
  "age": "number (required)"
}
```

## Setup and Run

1. Clone the repository
2. Install dependencies
```bash
npm install
```
3. Create a `.env` file in the root directory
PORT=3000
DB_URI=your_mongodb_atlas_connection_string

4. Start the server
```bash
node server.js
```

## Features
- Full CRUD operations
- Input validation via Mongoose schema
- Environment-based configuration
- MongoDB Atlas integration
- Proper HTTP status codes and error responses

