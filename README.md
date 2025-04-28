📖 Table of Contents
About the Project

Tech Stack

Project Structure

Getting Started

Available Scripts

API Endpoints

Screenshots

License

📝 About the Project
This project is a basic CRUD web application to manage employee records.
It allows users to:

Add new employees

View a list of all employees

Update existing employee details

Delete employees

Data is stored in MongoDB (Local Database) and managed with Mongoose ORM.
The frontend uses Axios to communicate with the backend APIs.

⚙️ Tech Stack
Frontend:

React.js

Axios

HTML, CSS

Backend:

Node.js

Express.js

MongoDB (Local) with Mongoose

Others:

Dotenv for environment variables

CORS for cross-origin communication

Nodemon for auto-reload backend server

🗂️ Project Structure
plaintext
Copy
Edit
employee-crud-backend/
 ├── models/
 │   └── Employee.js          # Mongoose Schema
 ├── routes/
 │   └── employeeRoutes.js    # All API routes
 ├── server.js                 # Entry point
 └── .env                      # MongoDB URI

employee-crud-frontend/
 └── src/
     └── App.js               # Frontend CRUD logic
🚀 Getting Started
Prerequisites
Node.js installed

MongoDB installed locally

npm installed

1. Clone the repository
bash
Copy
Edit
git clone https://github.com/your-username/employee-crud-mern.git
cd employee-crud-mern
2. Setup Backend
bash
Copy
Edit
cd employee-crud-backend
npm install
Create a .env file:

env
Copy
Edit
MONGO_URI=mongodb://127.0.0.1:27017/employeesDB
PORT=5000
Start MongoDB server locally:

bash
Copy
Edit
mongod
Start backend server:

bash
Copy
Edit
npm start
✅ Backend running on http://localhost:5000/

3. Setup Frontend
bash
Copy
Edit
cd ../employee-crud-frontend
npm install
npm start
✅ Frontend running on http://localhost:3000/

🖥️ Available Scripts
Backend:

bash
Copy
Edit
npm start         # Start backend server using nodemon
Frontend:

bash
Copy
Edit
npm start         # Start React development server
📡 API Endpoints

Method	Route	Description
POST	/api/employees/	Create a new employee
GET	/api/employees/	Get all employees
PUT	/api/employees/:id	Update an employee by ID
DELETE	/api/employees/:id	Delete an employee by ID# MERN-Project
