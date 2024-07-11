# To-Do List Application

This is a simple To-Do List application built with React, Node.js, and MongoDB. The application allows users to create, view, update, and delete tasks. Tasks can be marked as completed, and each task has a title, description, due date, and status.

## Features

- Create new tasks with a title, description, status, and due date.
- View a list of tasks.
- Edit task details.
- Delete tasks.
- Mark tasks as completed.

## Setup and Installation

### Prerequisites

- Node.js and npm installed on your machine.
- A MongoDB Atlas account (or a local MongoDB instance).

### Project Setup

1. **Clone the repository:**

    ```bash
    git clone https://github.com/your-username/todo-list-app.git
    cd todo-list-app
    ```

2. **Install dependencies for the server:**

    ```bash
    cd server
    npm install
    ```

3. **Install dependencies for the client:**

    ```bash
    cd ../client
    npm install
    ```

4. **Set up MongoDB Atlas:**

    - Create a MongoDB Atlas account and set up a new cluster.
    - Create a database user with read and write permissions.
    - Whitelist your IP address.
    - Get your MongoDB connection string.

5. **Configure the server to connect to MongoDB Atlas:**

    - Open `server/server.js` and replace the connection string with your MongoDB Atlas connection string.

    ```javascript
    const dbURI = "mongodb+srv://<username>:<password>@cluster0.mongodb.net/<dbname>?retryWrites=true&w=majority";
    ```

### Running the Application

1. **Start the server:**

    ```bash
    cd server
    node server.js
    ```

    The server should now be running on `http://localhost:3001`.

2. **Start the client:**

    ```bash
    cd ../client
    npm start
    ```

    The client should now be running on `http://localhost:3000`.

### API Endpoints

- `GET /getTodoList` - Retrieve the list of tasks.
- `POST /addTodoList` - Add a new task.
- `POST /updateTodoList/:id` - Update an existing task.
- `DELETE /deleteTodoList/:id` - Delete a task.

## Folder Structure

- `client` - Contains the React front-end code.
- `server` - Contains the Node.js back-end code.
- `models` - Contains the Mongoose models for MongoDB.

## UI
![image](https://github.com/malsha11/MERN-ToDo-Application/assets/84215169/b60ad823-ddc7-43b8-9364-2910394a1692)



