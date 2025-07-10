**Chat App**
================

**Table of Contents**
-----------------

1. [Overview](#overview)
2. [Tech Stack](#tech-stack)
3. [System Architecture](#system-architecture)
4. [How to Run](#how-to-run)
5. [API Endpoints](#api-endpoints)
6. [Socket.IO Events](#socketio-events)
7. [Frontend Components](#frontend-components)

**Overview**
------------

This is a real-time chat application built using a microservices architecture. The application consists of two main components: a backend API server (`chat-backend`) and a frontend client (`chat-frontend`).

**Tech Stack**
--------------

* **Backend:**
	+ Node.js
	+ Express.js
	+ Socket.IO
	+ MongoDB (using Mongoose)
	+ Cloudinary (for image storage)
	+ bcryptjs (for password hashing)
	+ jsonwebtoken (for authentication)
* **Frontend:**
	+ React.js
	+ Redux (using Zustand)
	+ React Router
	+ Webpack (using Vite)
	+ Axios (for API requests)
	+ React Hot Toast (for toast notifications)
	+ Lucide React (for icons)
* **Other:**
	+ dotenv (for environment variables)
	+ nodemon (for development)

**System Architecture**
----------------------

The application is designed as a microservices architecture, with separate services for the backend API and frontend client.

* **Backend API (`chat-backend`):**
	+ Handles user authentication and authorization
	+ Manages user data and chat messages
	+ Provides real-time updates using Socket.IO
* **Frontend Client (`chat-frontend`):**
	+ Handles user interface and user experience
	+ Makes API requests to the backend API
	+ Updates the UI in real-time using Socket.IO

**How to Run**
--------------

### Backend API (`chat-backend`)

1. Clone the repository and navigate to the `chat-backend` directory.
2. Install dependencies using `npm install`.
3. Start the server using `npm run dev`.
4. The server will start on port 3000.

### Frontend Client (`chat-frontend`)

1. Clone the repository and navigate to the `chat-frontend` directory.
2. Install dependencies using `npm install`.
3. Start the development server using `npm run dev`.
4. The client will start on port 5173.

**API Endpoints**
----------------

The backend API provides the following endpoints:

* **GET /api/auth/check**: Checks if the user is authenticated.
* **POST /api/auth/signup**: Creates a new user account.
* **POST /api/auth/login**: Logs in an existing user.
* **GET /api/messages/users**: Retrieves a list of online users.
* **GET /api/messages/:id**: Retrieves a list of messages for a specific user.
* **POST /api/messages/send/:id**: Sends a new message to a specific user.

**Socket.IO Events**
--------------------

The backend API emits the following Socket.IO events:

* **getOnlineUsers**: Emits a list of online users.
* **newMessage**: Emits a new message to the recipient.

**Frontend Components**
----------------------

The frontend client consists of the following components:

* **Navbar**: Handles user navigation and authentication.
* **ChatContainer**: Handles the chat interface and message rendering.
* **MessageInput**: Handles message input and sending.
* **SettingsPage**: Handles user settings and profile management.
* **ProfilePage**: Handles user profile management.

I hope this helps! Let me know if you need any further assistance.