# 🏛️ TenderAnalyser — REST API Microservice

The backend service powering the **TenderAnalyser** ecosystem. Built with Python and Flask, containerized via Docker, and deployed on Render. It handles business logic, bid evaluation state machines, document metadata, and competitive financial analytics.

> 🔗 **Frontend Repository:** Looking for the Android app? Check out the [TenderAnalyser Frontend Kotlin](https://github.com/aravinth016/TenderAnalyser-Frontend-Kotlin).

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
2. Create and activate virtual environment:

   Bash
   python3 -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
 
3. Install dependencies:

   Bash
   pip install -r requirements.txt
  
4.Environment Configuration:

   Create a local .env file in the root directory:
   Code snippet:
     FLASK_ENV=development
     SECRET_KEY=your_secret_key_here
    
5. Run the server:

    Bash
    
     python app.py
     The API server will start at http://127.0.0.1:5000/.

6.🐳 Running with Docker
    To build and run the backend locally using Docker:

   Bash
    # Build Docker image
    docker build -t tender-analyser-backend .
    
    # Run Docker container
    docker run -p 5000:5000 tender-analyser-backend
