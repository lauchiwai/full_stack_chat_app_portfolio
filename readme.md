# 🚀 Full-Stack Real-Time Communication & Learning Platform

This is a full-stack project independently developed by me, integrating real-time chat, language learning (vocabulary/articles), and AI Q&A functionality. The project adopts a microservices architecture, demonstrating comprehensive skills from frontend, backend to DevOps.

## 📁 Project Architecture & Repository Links

The project consists of three core services. Click the links to view detailed code and documentation for each service:

| Service Name | Tech Stack | Repository Link | Core Features |
| :--- | :--- | :--- | :--- |
| **Main Backend Service** | .NET 8, MSSQL, RabbitMQ, Docker | [dotnet_chatroom_service](https://github.com/lauchiwai/dotnet_chatroom_service) | User Authentication, Vocabulary Management, Article Management, Chat Rooms, Outbox Pattern |
| **AI Chat Service** | FastAPI, MongoDB, Qdrant, Docker | [py_chat_service](https://github.com/lauchiwai/py_chat_service) | Chat History Storage, RAG AI Q&A, Vector Search |
| **Frontend Application** | Vue 3, TypeScript, Pinia, Docker | [vue_chatroom_service](https://github.com/lauchiwai/vue_chatroom_service) | Responsive Web Design, Real-time Communication, Learning Features, Dual Token Authentication, CSP |

| Item | Link | Account Information |
| :--- | :--- | :--- |
| **Frontend Application (Vue.js)** | [https://oniind244.online/](https://oniind244.online/) |  |
| **Demo Video** | [https://www.youtube.com/shorts/KFJzDUnJtvw](https://www.youtube.com/shorts/KFJzDUnJtvw) |  |
| **Test Account 1** | | **Username:** `user01` <br> **Password:** `a1234*` |
| **Test Account 2** | | **Username:** `` <br> **Password:** `` |

## 🛠️ Technical Highlights

### 🔐 Security & Architecture
- **Dual JWT Authentication System**: Implemented Access Token and Refresh Token mechanism to ensure user security and seamless refresh.
- **Microservices Communication**: Main backend service communicates asynchronously with AI service through message queue (RabbitMQ), achieving service decoupling.
- **Outbox Pattern**: Ensures eventual consistency between database updates and message delivery in distributed systems.

### ⚡ Real-time & User Experience
- **Server-Sent Events (SSE)**: Used for real-time data push, providing smooth user experience.
- **RAG AI Q&A**: Combined Qdrant vector database with FastAPI to create an intelligent Q&A bot based on custom knowledge base.
- **Responsive Web Design (RWD)**: Frontend uses Vue 3 and SCSS to ensure perfect experience on mobile, tablet, and desktop.

### 🚀 Deployment & Operations (DevOps)
- **Containerization**: All services are containerized using Docker for easy development, testing, and deployment.
- **CI/CD Pipeline**: Established automated build, test, and deployment pipelines for each service.
- **Content Security Policy (CSP)**: Implemented CSP headers on frontend to effectively defend against XSS and other web attacks.
