# To-Do Web Application

A full-stack To-Do Web Application built using HTML, CSS, JavaScript, Node.js, Express.js, and PostgreSQL. The application allows users to create accounts, securely log in, manage their personal tasks, and track task completion through an interactive dashboard.

## Features

- **User Registration:** Create an account with name, email, and password.
- **User Login:** Authenticate users using their registered credentials.
- **Dashboard:** View and manage personal tasks.
- **Add Tasks:** Create new to-do items.
- **View Tasks:** Display all added tasks.
- **Edit Tasks:** Update existing task details.
- **Delete Tasks:** Remove unwanted tasks.
- **Task Status:** Mark tasks as pending or completed.
- **User Authentication:** Protect user accounts and task data.
- **Data Persistence:** Store user information and tasks in PostgreSQL.

## Technologies Used

### Frontend
- HTML5
- CSS3
- JavaScript

### Backend
- Node.js
- Express.js

### Database
- PostgreSQL

### Libraries and Tools
- pg
- bcryptjs
- jsonwebtoken
- dotenv
- cors
- cookie-parser
- Nodemon
- Git and GitHub
- Postman

## Project Structure

```text
todo-web-app/
│
├── client/
│   ├── index.html
│   ├── signup.html
│   ├── dashboard.html
│   │
│   ├── css/
│   │   ├── style.css
│   │   ├── auth.css
│   │   └── dashboard.css
│   │
│   ├── js/
│   │   ├── api.js
│   │   ├── auth.js
│   │   ├── signup.js
│   │   └── todo.js
│   │
│   └── assets/
│       └── images/
│
├── server/
│   ├── src/
│   │   ├── config/
│   │   │   └── db.js
│   │   │
│   │   ├── controllers/
│   │   │   ├── authController.js
│   │   │   └── todoController.js
│   │   │
│   │   ├── middleware/
│   │   │   └── authMiddleware.js
│   │   │
│   │   ├── routes/
│   │   │   ├── authRoutes.js
│   │   │   └── todoRoutes.js
│   │   │
│   │   ├── utils/
│   │   │   └── tokenUtils.js
│   │   │
│   │   └── server.js
│   │
│   ├── .env
│   ├── .env.example
│   ├── .gitignore
│   ├── package.json
│   └── package-lock.json
│
├── database/
│   └── schema.sql
│
└── README.md
```

## Installation and Setup

### Prerequisites

Make sure you have installed:

- Node.js
- npm
- PostgreSQL
- Git

### 1. Clone the Repository

```bash
git clone <your-repository-url>
```

### 2. Navigate to the Project

```bash
cd todo-web-app
```

### 3. Install Backend Dependencies

```bash
cd server
npm install
```

### 4. Configure Environment Variables

Create a `.env` file inside the server directory and configure the following variables:

```env
PORT=5000
DB_HOST=localhost
DB_PORT=5432
DB_NAME=todo_db
DB_USER=postgres
DB_PASSWORD=your_database_password
JWT_SECRET=your_secret_key
CLIENT_URL=http://localhost:5500
```

### 5. Configure the Database

Create a PostgreSQL database named `todo_db` and execute the SQL commands provided in:

```text
database/schema.sql
```

### 6. Start the Backend Server

From the server directory, run:

```bash
npm run dev
```

The backend server will run at:

```text
http://localhost:5000
```

### 7. Run the Frontend

Open the frontend using the VS Code Live Server extension or another local static server.

## Application Modules

### 1. Authentication Module
- User registration
- User login
- Password hashing
- Authentication and authorization
- Logout

### 2. Task Management Module
- Create tasks
- View tasks
- Update tasks
- Delete tasks
- Update task completion status

### 3. Dashboard Module
- Display user information
- View personal task list
- Track pending and completed tasks
- Manage tasks through the dashboard

## Future Improvements

- Task priority management
- Due dates and reminders
- Search and filter functionality
- Task categories
- Responsive mobile-friendly interface

## License

This project is licensed under the MIT License.

## In Progress...