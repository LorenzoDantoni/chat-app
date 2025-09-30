# Full Stack Real-Time Chat Application

This is a full-stack, real-time chat application built with the **MERN** stack (MongoDB, Express, React, Node.js) and **Socket.IO**.

## Project Description

This application allows users to register, login, and chat with other users in real-time. When a user sends a message, it is instantly delivered to the recipient without the need to reload the page. This is achieved using Socket.IO, which enables bidirectional communication between the client and the server.

The application is divided into two main parts:

*   **Client:** A React application that provides the user interface for the chat.
*   **Server:** A Node.js and Express application that handles user authentication, message storage, and real-time communication.

## Technologies Used

### Backend

*   **Node.js:** A JavaScript runtime environment for executing server-side code.
*   **Express:** A web application framework for Node.js, used to build the REST APIs.
*   **MongoDB:** A NoSQL database used to store user information and chat messages.
*   **Mongoose:** An Object Data Modeling (ODM) library for MongoDB and Node.js.
*   **Socket.IO:** A library that enables real-time, bidirectional and event-based communication between the browser and the server.
*   **JSON Web Token (JWT):** For securing the REST APIs.
*   **bcryptjs:** For hashing user passwords before storing them in the database.
*   **Cloudinary:** For storing user profile pictures.

### Frontend

*   **React:** A JavaScript library for building user interfaces.
*   **React Router:** For handling client-side routing.
*   **Socket.IO Client:** The client-side library for Socket.IO.
*   **Axios:** A promise-based HTTP client for making requests to the backend.
*   **Vite:** A build tool that provides a faster and leaner development experience for modern web projects.
*   **Tailwind CSS:** A utility-first CSS framework for styling the application.
*   **React Hot Toast:** For displaying notifications.

## Features

*   User registration and login
*   Real-time messaging
*   Online status for users
*   Unread message count
*   Profile picture upload

## Getting Started

### Prerequisites

*   Node.js (v14 or later)
*   MongoDB Atlas account or a local MongoDB instance
*   Cloudinary account

### Installation

1.  **Clone the repository:**

    ```bash
    git clone https://github.com/your-username/chat-app.git
    cd chat-app
    ```

2.  **Install server dependencies:**

    ```bash
    cd server
    npm install
    ```

3.  **Install client dependencies:**

    ```bash
    cd ../client
    npm install
    ```

### Configuration

1.  **Create a `.env` file in the `server` directory** and add the following environment variables:

    ```
    PORT=5000
    MONGO_URI=<your_mongodb_uri>
    JWT_SECRET=<your_jwt_secret>
    CLOUDINARY_CLOUD_NAME=<your_cloudinary_cloud_name>
    CLOUDINARY_API_KEY=<your_cloudinary_api_key>
    CLOUDINARY_API_SECRET=<your_cloudinary_api_secret>
    ```

2.  **Create a `.env` file in the `client` directory** and add the following environment variable:

    ```
    VITE_API_URL=http://localhost:5000
    ```

### Running the Application

1.  **Start the server:**

    ```bash
    cd server
    npm run server
    ```

2.  **Start the client:**

    ```bash
    cd ../client
    npm run dev
    ```
