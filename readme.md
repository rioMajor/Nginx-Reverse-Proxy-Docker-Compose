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

### ❓FAQs

**Q: Is this a full-time role?**
Yes. You would need to be in office in Bangalore.

**Q: Is there a stipend?**
Yes. 20k INR per month

**Q: How many positions are open?**
Two positions are open.

**Q: I am still in college. Can I apply?**
Unfortunately, we are looking for post-college candidates.

**Q: Can I reach out for doubts?**
No — due to the volume of submissions. Please use your creativity and assumptions where needed.

**Q: Can I use ChatGPT or Copilot?**
Yes, feel free to use AI tools — we care about your implementation and understanding.

**Q: This feels like a lot for an intern assignment.**
We agree it’s non-trivial — we’ve received many applications, so this helps us filter based on quality.


