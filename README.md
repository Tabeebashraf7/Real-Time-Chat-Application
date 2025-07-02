💬 Real-Time Chat Application using Node.js & Socket.IO

A Real-Time Chat Application built using Node.js and Socket.IO, enabling multiple users to communicate simultaneously in a dynamic environment. The app supports real-time message exchange, emoji support, audio notifications, and user join/leave alerts.

🚀 Features

🔁 Real-time Communication via WebSocket using Socket.IO

👥 Multi-user Support for simultaneous chat participation

🛎️ Notifications when a user joins or leaves the room

🔔 Sound Alerts for message send/receive and disconnections

😀 Emoji Support in messages

💻 Client-Server Architecture with a separate Node.js server and frontend client

🧠 How It Works

WebSocket Protocol is used for real-time, two-way communication between the client and server.

Built using Node.js with Socket.IO to handle connections and broadcast events.

A dedicated Node.js server listens to all socket events.

The client-side is a standalone web page that connects to the Node server via a script:

html
Copy
Edit
<script src="http://localhost:8000/socket.io/socket.io.js"></script>
🗂️ Project Structure

pgsql
Copy
Edit
chat-app/
├── node-server/
│   ├── index.js         - Main Node.js socket server
│   └── package.json     - Node dependencies
├── client/
│   ├── index.html       - Frontend page with chat UI
│   └── client.js        - Socket logic on the client side
⚙️ Installation & Setup

1️⃣ Backend (Node Server)

bash
Copy
Edit
cd node-server
npm init -y
npm install socket.io
2️⃣ Client

No major setup needed — simply open client/index.html in your browser after starting the server.

▶️ Running the App

Start your Node server (make sure it's running on port 8000 or update the client accordingly):

bash
Copy
Edit
node index.js
Open the index.html file in any browser:

bash
Copy
Edit
client/index.html
You're ready to chat in real time!

📄 index.js (Node Server Overview)

Initializes the socket connection

Listens for user connections and messages

Broadcasts join/leave events and chat messages to all connected users

📄 client.js (Client Overview)

Connects to the server using socket.io.js

Sends user messages

Plays sound on message received/sent

Handles emoji input and updates UI dynamically

🔊 Audio & Emoji Support

Sound files are triggered when a user:

Joins the room

Sends or receives a message

Leaves the chat

Emojis can be typed or selected using any emoji keyboard or picker plugin.

🧪 Future Improvements

✅ User authentication and login system

📜 Chat history with database (MongoDB or Firebase)

📷 Media sharing (images, videos)

🌐 Room-based chat support

💬 Typing indicator

🤝 Contributing

Feel free to fork the repo and contribute to making this chat app even better! Just create a pull request with your updates and features.
