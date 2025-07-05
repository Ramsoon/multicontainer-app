## multicontainer-app - Full-Stack Node.js App with Docker, Networking & Persistent Volumes

This project demonstrates a complete Dockerized full-stack Node.js application, separating the frontend, backend, and MongoDB services into individual containers. These services communicate via a shared Docker network, and MongoDB leverages persistent volumes to ensure data is not lost when containers are stopped or removed.
 🧱 Architecture

 📦 Services

Frontend: A web interface (built with HTML/CSS/JS or React) served via  Node.js
Backend: Node.js + Express API handling HTTP requests and communicating with MongoDB
Database: MongoDB 4.4 containerized with authentication and volume-based data persistence

 🔌 Networking

 A custom Docker network (`goalsnet`) enables inter-container communication without exposing unnecessary ports
 DNS resolution is handled internally, allowing services to use names like `mongodb` and `backend` to connect

 💾 Data Persistence

- MongoDB uses a named volume (`mongo_data`) to store data
- Demonstrates both named volumes and bind mounts for development flexibility


 🧰 Technologies Used

- Node.js / Express – Backend RESTful API
- MongoDB – NoSQL database
- Docker / Docker Compose – Containerization & orchestration
- React , HTML/CSS – Frontend application


 📦 Usage

1. Clone the repo
2. Build and start all services
 for the backend, expose port 80 on your Dockerfile and 3000 for your frontend Dockerfile then access via localhost on your web browser

 📚 Learning Highlights

- Isolating services using containers
- Dockerizing full-stack applications
- Secure database communication with credentials
- Volume-based MongoDB persistence
- Container-to-container networking

 🤝 Contributions

Pull requests are welcome. For major changes, please open an issue first to discuss what you'd like to change.

📝 License

This project is open-source and available under the [MIT License](LICENSE).

