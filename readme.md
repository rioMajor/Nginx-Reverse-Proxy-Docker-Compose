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

### 📦 Tech Constraints

* Nginx must run in a Docker container, not on host
* Use bridge networking (no host networking)

---

### 📝 Submission Instructions

1. Upload your project to GitHub or GitLab.
2. Include a short `README.md` with:

   * Setup instructions
   * How routing works
   * Any bonus you implemented
3. Deadline: **1 week**
4. Bonus points for:

   * Logging clarity
   * Clean and modular Docker setup
   * Healthcheck or automated test script

---



