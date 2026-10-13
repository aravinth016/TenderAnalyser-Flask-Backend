# 🏛️ TenderAnalyser — REST API Microservice

The backend service powering the **TenderAnalyser** ecosystem. Built with Python and Flask, containerized via Docker, and deployed on Render. It handles business logic, bid evaluation state machines, document metadata, and competitive financial analytics.

> 🔗 **Frontend Repository:** Looking for the Android app? Check out the [TenderAnalyser Android App](https://github.com/aravinth016/TenderAnalyser-Frontend-Kotlin).

---

## 🌟 Key Features

* **RESTful API Endpoints:** Complete API suite handling user authentication, tender publishing, bid submissions, and withdrawal workflows.
* **Post-Bidding Evaluation Engine:** Handles dynamic status transitions (`Pending Review`, `Evaluating`, `Awarded`, `Not Awarded`) and dynamic feedback generation.
* **Financial Analytics Services:** Computes bidder rankings, calculates L1 pricing differences, and generates competitive market averages for post-bidding analysis.
* **Containerized Deployment:** Dockerized setup for consistent production deployments on Render Cloud Services.

---

## 🛠️ Tech Stack

* **Language:** Python 3.12
* **Framework:** Flask / Flask-CORS
* **WSGI Server:** Gunicorn
* **Containerization:** Docker
* **Deployment Platform:** Render

---

## 📁 Repository Structure

.
├── app.py              # Flask app entry point & API route handlers
├── Dockerfile          # Docker container specifications
├── .dockerignore       # Docker build exclusion rules
├── requirements.txt    # Python dependency manifest
└── README.md           # Repository documentation


---

## 🚀 Local Setup & Development

### Prerequisites
* Python 3.12+
* Virtualenv (`venv`)

### Setup Instructions
1. **Clone the repository:**
   ```bash
   git clone [https://github.com/aravinth016/TenderAnalyser-Backend.git](https://github.com/aravinth016/TenderAnalyser-Backend.git)
   cd TenderAnalyser-Backend
