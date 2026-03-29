# 🚀 Real-Time Chat Application

A scalable, real-time chat application built using Java, Spring Boot, Angular, Kafka, and Redis, designed to handle high concurrency and low-latency messaging.

---

## 📌 Features

- 🔹 Real-time messaging using WebSockets  
- 🔹 1:1 and group chat support  
- 🔹 User online/offline presence tracking  
- 🔹 Message persistence and chat history  
- 🔹 Read receipts and typing indicators  
- 🔹 Event-driven architecture using Kafka  
- 🔹 Redis caching for performance optimization  
- 🔹 Secure authentication using JWT  
- 🔹 Cloud deployment on AWS  

---

## 🏗️ Architecture

Frontend (Angular) communicates with backend services via API Gateway.  
WebSocket-based Chat Service handles real-time communication.  
Kafka is used for asynchronous message processing.  
Redis is used for caching and user presence.  
Messages are stored in a relational database.

---

## ⚙️ Tech Stack

Backend: Java, Spring Boot, Spring WebSocket  
Frontend: Angular, TypeScript  
Messaging: Apache Kafka  
Caching: Redis  
Database: MySQL / PostgreSQL  
Cloud: AWS (EC2, S3, RDS)  
Tools: Maven, Git, Docker (optional)  

---

## 🔄 Message Flow

1. User sends message via WebSocket  
2. Chat Service publishes event to Kafka  
3. Message Service consumes event and stores it in DB  
4. Chat Service delivers message to recipient in real-time  
5. If user is offline, message is stored and delivered later  

---

## 📂 Project Structure

chat-app/
├── frontend-angular/
├── api-gateway/
├── auth-service/
├── chat-service/
├── message-service/
├── docker-compose.yml
└── README.md

---

## 🚀 Getting Started

### Prerequisites
- Java 17+
- Node.js & Angular CLI
- Kafka & Zookeeper
- Redis
- MySQL/PostgreSQL

### Run Locally

1. Clone the repository  
2. Start Kafka, Redis, and Database  
3. Run backend services using Maven  
4. Start Angular frontend  
5. Access application at http://localhost:4200  

---

## 📊 Future Enhancements

- Push notifications  
- Media/file sharing  
- End-to-end encryption  
- Kubernetes deployment  

---

## 💡 Key Highlights

- Built using microservices architecture  
- Implemented event-driven system using Kafka  
- Optimized performance using Redis caching  
- Designed for scalability and high availability  

---

## 👨‍💻 Author

Awiral
