# CRUD API Application

A RESTful API for performing CRUD operations on user data using Express.js and MongoDB.

## API Endpoints

| Method | Endpoint | Description |
|--------|----------|-------------|
| GET | `/api/users` | Get all users |
| GET | `/api/users/:id` | Get user by ID |
| POST | `/api/users` | Create new user |
| PUT | `/api/users/:id` | Update user |
| DELETE | `/api/users/:id` | Delete user |

## User Schema
```json
{
  "name": "string (required)",
  "email": "string (required, unique)",
  "age": "number (required)",
  "city": "string (required)"
}
```

## Installation
```bash
npm install
npm start
```

## Testing with Postman

### 1. Create User (POST)
- URL: `https://your-app.onrender.com/api/users`
- Method: POST
- Body (JSON):
```json
{
  "name": "John Doe",
  "email": "john@example.com",
  "age": 25,
  "city": "New York"
}
```

### 2. Get All Users (GET)
- URL: `https://your-app.onrender.com/api/users`
- Method: GET

### 3. Get User by ID (GET)
- URL: `https://your-app.onrender.com/api/users/{user_id}`
- Method: GET

### 4. Update User (PUT)
- URL: `https://your-app.onrender.com/api/users/{user_id}`
- Method: PUT
- Body (JSON):
```json
{
  "name": "John Smith",
  "age": 26
}
```

### 5. Delete User (DELETE)
- URL: `https://your-app.onrender.com/api/users/{user_id}`
- Method: DELETE