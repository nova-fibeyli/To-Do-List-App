# To-Do List Application

## Description

The **To-Do List Application** is a simple and efficient task management API built using **Node.js**, **Express.js**, and **MongoDB**. It allows users to create, update, retrieve, and delete tasks, making it an excellent starting point for learning **REST API development** and **MongoDB integration**.

## Table of Contents

- [Installation](#installation)
- [Usage](#usage)
- [Features](#features)
- [API Endpoints](#api-endpoints)
- [Postman Instructions](#postman-instructions)
- [MongoDB Compass Usage](#mongodb-compass-usage)
- [Contributing](#contributing)

## Installation

Follow these steps to set up the project locally:

1. **Clone the Repository**
   ```sh
   git clone https://github.com/your-repo/todo-app.git
   cd todo-app
   ```
2. **Install Dependencies**
   ```sh
   npm install
   ```
3. **Start MongoDB** (if running locally)
   ```sh
   mongod
   ```
4. **Run the Server**
   ```sh
   node index.js
   ```
   The server should start at `http://localhost:5000`

## Usage

Once the server is running, you can interact with the API using **Postman** or **MongoDB Compass**.

### Postman Instructions

Use **Postman** to send HTTP requests:

- **Create a Task:**
  - Method: `POST`
  - URL: `http://localhost:5000/tasks`
  - Body:
    ```json
    {
      "title": "My first task"
    }
    ```
- **Retrieve Tasks:**
  - Method: `GET`
  - URL: `http://localhost:5000/tasks`
- **Update a Task:**
  - Method: `PUT`
  - URL: `http://localhost:5000/tasks/{task_id}`
  - Body:
    ```json
    {
      "completed": true
    }
    ```
- **Delete a Task:**
  - Method: `DELETE`
  - URL: `http://localhost:5000/tasks/{task_id}`

### MongoDB Compass Usage

1. Open **MongoDB Compass**.
2. Connect to `mongodb://localhost:27017/todoDB`.
3. Browse the `tasks` collection to view, insert, update, or delete records.

## Features

- **Task Management**: Create, read, update, and delete tasks.
- **RESTful API**: Well-structured API endpoints.
- **MongoDB Integration**: Uses Mongoose for database operations.
- **Error Handling**: Proper error messages for invalid requests.
- **CORS Enabled**: Allows API calls from different origins.

## Contributing

Feel free to contribute by submitting a **pull request** or opening an **issue**.

---

Happy coding! 🚀
