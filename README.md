# Student Grading System (Node.js, Express)

Simple student grading system using Node.js and Express.
Provides REST API endpoints to create/read/update/delete students and compute averages.

## Requirements
- Node.js 18+ (or compatible)
- npm

## Install
```bash
npm install
```

## Run
```bash
npm start
```

The server will run on port 3000 by default.

## API Endpoints
- `GET /students` - List all students
- `GET /students/:id` - Get student by id
- `POST /students` - Create a student
    - body: `{ "name": "Alice", "grades": [85,90,78] }`
- `PUT /students/:id` - Update student (name/grades)
- `DELETE /students/:id` - Delete student
- `GET /students/:id/average` - Get average grade for a student
- `GET /grades/average` - Get class average

## Notes
- This is a simple in-memory example. Data is stored in `data/students.json`.
- For production, connect a real database (MongoDB, Postgres, etc.)
