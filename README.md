


# Affinity Website

Affinity is a platform designed for people to connect with others of similar intellectual levels. This repository contains the full stack of the project, including the frontend, backend, AI chat server, real chat server, Rust server, machine learning model for AI chat, and socket implementations for real-time communication and WebRTC.

Hosted Website : [http://ec2-13-126-149-80.ap-south-1.compute.amazonaws.com:5173/]

## Project Structure

The repository is organized into the following main folders:

1. **Client Vite React**
2. **AI Chat Server**
3. **Real Chat Server**
4. **Rust Server**
5. **DateHer Model**
6. **Socket For RealChat**
7. **Socket for WebRTC**

### 1. Client Vite React

The client folder contains the frontend code built using React and Vite. The client is responsible for rendering the user interface and handling user interactions. Key features include:

- **Modern UI/UX**: Built using Tailwind CSS and Framer Motion for smooth animations and responsiveness.
- **User Authentication**: Integration with the backend for user login and registration.
- **Profile Matching**: Displays profiles of users with similar intellectual levels.
- **Real-time Chat Interface**: Allows users to chat with matched profiles in real-time.
- **WebRTC for Video Calls**: Facilitates video calls between matched users using WebRTC.

### 2. AI Chat Server

The AI Chat Server is responsible for handling AI-driven conversations between users and an AI chatbot. Key components include:

- **Natural Language Processing (NLP)**: Utilizes machine learning models to generate meaningful responses.
- **API Endpoints**: Exposes endpoints for the client to interact with the AI chatbot.
- **Session Management**: Tracks user sessions and provides contextual responses.

### 3. Real Chat Server

The Real Chat Server handles real-time communication between users. Key features include:

- **Message Handling**: Supports sending and receiving text messages between users.
- **Database Integration**: Stores chat history for future reference.
- **User Presence Tracking**: Monitors online/offline status of users.
- **Scalability**: Designed to handle multiple chat sessions concurrently.

### 4. Rust Server

The Rust Server is responsible for performance-critical operations that require low latency and high throughput. It handles tasks such as:

- **Data Processing**: Performs intensive data processing tasks efficiently.
- **API Gateway**: Acts as an intermediary for other services, ensuring fast and secure communication.
- **Real-Time Analytics**: Processes and delivers real-time analytics data to the client.

### 5. DateHer Model

This folder contains the machine learning model used for AI-driven chats. The model is trained on a dataset of conversations and is designed to:

- **Understand User Input**: Leverages NLP techniques to parse and understand user queries.
- **Generate Responses**: Produces contextually appropriate responses based on the conversation history.
- **Customization**: Allows for fine-tuning to adapt to different conversation styles.

### 6. Socket For RealChat

The Socket Server for Real Chat handles real-time communication using WebSockets. Key functionalities include:

- **Bi-directional Communication**: Enables real-time chat functionality between users.
- **Scalability**: Supports multiple concurrent users with minimal latency.
- **Event Handling**: Manages events like user typing, message delivery, and read receipts.

### 7. Socket for WebRTC

This folder contains the socket implementation for WebRTC, which powers the real-time video and audio communication between users. Key features include:

- **Peer-to-Peer Communication**: Establishes direct connections between users for video calls.
- **Signaling Server**: Facilitates the initial connection setup between peers.
- **Media Stream Handling**: Manages the transmission of audio and video streams during the call.
- **Error Handling**: Ensures smooth video calls by managing network interruptions and other issues.

## Getting Started

### Prerequisites

Before you begin, ensure you have the following installed:

- Node.js (v14.x or later)
- Rust (v1.54.0 or later)
- Python (for ML model)
- WebRTC-compatible browser

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/affinity.git
   cd affinity
   ```

2. Install dependencies for the client:
   ```bash
   cd client-vite-react
   npm install
   ```

3. Set up the servers:
   - For AI Chat Server:
     ```bash
     cd ai-chat-server
     npm install
     ```
   - For Real Chat Server:
     ```bash
     cd real-chat-server
     npm install
     ```
   - For Rust Server:
     ```bash
     cd rust-server
     cargo build
     ```
   - For Socket Servers:
     ```bash
     cd socket-for-realchat
     npm install
     ```
   - For Machine Learning Model:
     ```bash
     cd dateher-model
     pip install -r requirements.txt
     ```

### Running the Application

1. Start the client:
   ```bash
   cd client-vite-react
   npm run dev
   ```

2. Start the AI Chat Server:
   ```bash
   cd ai-chat-server
   npm start
   ```

3. Start the Real Chat Server:
   ```bash
   cd real-chat-server
   npm start
   ```

4. Start the Rust Server:
   ```bash
   cd rust-server
   cargo run
   ```

5. Start the Socket Servers:
   ```bash
   cd socket-for-realchat
   npm start
   ```

6. Start the Machine Learning Model:
   ```bash
   cd dateher-model
   python model.py
   ```

### Contributing

We welcome contributions to enhance the Affinity platform. Please follow these steps to contribute:

1. Fork the repository.
2. Create a new branch (`git checkout -b feature/your-feature`).
3. Commit your changes (`git commit -m 'Add some feature'`).
4. Push to the branch (`git push origin feature/your-feature`).
5. Create a pull request.

### License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

### Contact

For any questions or support, please contact `affinity.srp@gmail.com`.
```
