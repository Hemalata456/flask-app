# Flask CI/CD Pipeline with Jenkins and Docker

This project contains a simple Python Flask application containerized with Docker and automated through a Jenkins CI/CD Pipeline.  
The pipeline performs the following steps:

1. **Checkout Code from GitHub**
2. **Build Docker Image**
3. **Run Tests**
4. **Deploy the Container on the Jenkins Server**


## 📁 Project Structure

flask-app/
│
├── app.py
├── requirements.txt
├── Dockerfile
└── Jenkinsfile

## 🚀 Flask Application

A minimal Flask app is included in `app.py`


🐳 Docker Setup

The Dockerfile defines how the Flask application is containerized.


🔧 Jenkins CI/CD Pipeline

The pipeline uses a declarative Jenkinsfile located in the repository.


we built a complete CI/CD setup for a simple Python Flask application.
We created a small Flask app, containerized it using Docker, and automated the entire build–test–deploy process using Jenkins.
Whenever code is pushed to GitHub, Jenkins automatically pulls the latest code, builds a Docker image, runs basic tests, and deploys the updated container on the server.

This demonstrates how modern DevOps pipelines work by combining GitHub → Jenkins → Docker → Deployment in one automated flow.


👤 **Author**

*Challa Hemalata*
DevOps Intern | Cloud Enthusiast

📧 hemalatach154@gmail.com
🐙 GitHub: @hemalata456