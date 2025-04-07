# MERN Stack CRUD Operations

This project demonstrates how to perform CRUD (Create, Read, Update, Delete) operations using the MERN stack (MongoDB, Express.js, React.js, and Node.js). It's based on a tutorial that guides you through building a simple application to manage user data.

## Project Structure

The project is organized into two main directories:

-   `client`: Contains the React.js front-end application.
-   `server`: Contains the Node.js/Express.js back-end API.

## Technologies Used

-   **Front-end:**
    -   React.js
    -   React Router DOM
    -   Axios (for API requests)
    -   Bootstrap (for styling)
-   **Back-end:**
    -   Node.js
    -   Express.js
    -   MongoDB (with Mongoose)
    -   Cors (for cross-origin resource sharing)

## Setup and Installation

### Back-end (Server)

1.  **Navigate to the server directory:**

    ```bash
    cd server
    ```

2.  **Initialize a new Node.js project:**

    ```bash
    npm init -y
    ```

3.  **Install dependencies:**

    ```bash
    npm install express mongoose cors
    ```

4.  **Configure MongoDB connection:**
    -   Ensure you have MongoDB installed and running.
    -   Update the connection string in `server/index.js` with your MongoDB URI.

5.  **Start the server:**

    ```bash
    node index.js
    ```

### Front-end (Client)

1.  **Navigate to the client directory:**

    ```bash
    cd ../client
    ```

2.  **Create a new React application:**

    ```bash
    npx create-react-app .
    ```

3.  **Install dependencies:**

    ```bash
    npm install react-router-dom axios bootstrap
    ```

4.  **Start the React application:**

    ```bash
    npm start
    ```

## Functionality

-   **Create User:** Allows users to add new user records through a form.
-   **Read Users:** Displays a list of all users fetched from the MongoDB database.
-   **Update User:** Enables users to edit existing user records.
-   **Delete User:** Provides functionality to remove user records from the database.

## API Endpoints

-   `POST /users`: Creates a new user.
-   `GET /users`: Retrieves all users.
-   `PUT /users/:id`: Updates a user by ID.
-   `DELETE /users/:id`: Deletes a user by ID.

## MongoDB Schema

The user data is stored in a MongoDB collection with the following schema:

```javascript
// Example (adjust as needed)
const userSchema = new mongoose.Schema({
  name: String,
  email: String,
  age: Number,
});
