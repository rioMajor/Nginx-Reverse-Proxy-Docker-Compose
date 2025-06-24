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

