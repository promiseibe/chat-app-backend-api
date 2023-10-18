# chat-app-backend-api
Chat Application Backend
This repository contains the backend code for a real-time chat application. The backend is built using Node.js, Express.js, Socket.IO, and MongoDB. It provides the necessary API endpoints and WebSocket functionality to enable real-time messaging between users.

Features
Real-time Messaging: Users can send and receive messages in real-time.
Multiple Rooms: Users can join different chat rooms and have group conversations.
User Management: Basic user authentication and status tracking (online/offline) are implemented.
Message History: Chat rooms store message history and deliver it to users when they join.
Technologies Used
Node.js: The backend is built on Node.js, a fast and scalable server-side JavaScript runtime.
Express.js: Express is used as the web application framework for Node.js, simplifying the creation of robust APIs.
Socket.IO: Socket.IO enables real-time, bidirectional, and event-based communication.
MongoDB: MongoDB is a NoSQL database used for storing user data and chat history.
Mongoose: Mongoose is an ODM (Object Data Modeling) library for MongoDB and Node.js.
RESTful API: The backend provides RESTful APIs for user authentication and chat room management.

Getting Started
Clone the Repository:
git clone https://github.com/promiseibe/chat-app-backend.git
cd chat-app-backend
Install Dependencies:
npm install

Set Up Environment Variables:
Create a .env file in the root directory with the following variables:
MONGODB_URI=mongodb://localhost:27017/chatapp
PORT=5001
Modify the MongoDB URI as per your MongoDB setup.

Start the Server:
npm start
The server will start on http://localhost:5001.

API Endpoints
POST /users/register: Register a new user. Requires username and password in the request body.
POST /users/login: Log in an existing user. Requires username and password in the request body.
GET /rooms: Get a list of available chat rooms.
Socket.IO Events:
connection: Handle new client connections.
new-user: Broadcast when a new user joins.
join-room: Handle when a user joins a specific chat room.
message-room: Handle new messages in chat rooms.
room-messages: Send chat room history to users when they join.
Contributing
Feel free to contribute to the development of this chat application by opening issues or pull requests. Your feedback and contributions are welcome!

