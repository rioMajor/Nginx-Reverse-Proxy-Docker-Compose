#  Nginx Reverse Proxy + Docker Compose (DevOps Assignment)

This project sets up two backend services (Go + Python) behind an Nginx reverse proxy using Docker Compose.

---

## 🛠 Setup Instructions

### 1. Clone the repository

```bash
git clone https://github.com/<your-username>/devops-nginx-docker.git
cd SourceCodeForDevopsAssignment
docker-compose up --build



.
├── docker-compose.yml
├── nginx/
│   ├── nginx.conf
│   └── Dockerfile
├── service_1/
│   ├── main.go
│   ├── Dockerfile
│   └── go.mod
├── service_2/
│   ├── app.py
│   └── Dockerfile
└── README.md

How Routing Works
This project uses Nginx as a reverse proxy to route incoming HTTP requests to the appropriate backend services based on the URL path. Nginx is configured to listen on port 8080, and all client requests are routed through it. Two backend services—one written in Go and the other in Python (Flask)—are each assigned their own internal ports (8001 and 8002, respectively).The routing logic is defined in the nginx.conf file, where:Any request with the path prefix /service1/ is forwarded to the Go service running on port 8001.Any request with the path prefix /service2/ is forwarded to the Python service running on port 8002.For example, a request to http://localhost:8080/service1/hello is internally redirected by Nginx to the Go container at http://service1:8001/hello. Similarly, http://localhost:8080/service2/hello is forwarded to the Flask app at http://service2:8002/hello.This is made possible because Docker Compose automatically connects all containers to a shared network and enables name-based service discovery. Nginx can access the backend containers using their service names (service1 and service2), ensuring smooth communication without requiring IP addresses.In short, the Nginx reverse proxy acts as a central gateway, making both services accessible from a single port (8080) while maintaining clean and modular routing based on URL paths.
