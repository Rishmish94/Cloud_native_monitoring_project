
# Cloud Native Resource Monitoring Python App on Kubernetes

## Overview
This project demonstrates my proficiency in building and deploying a Cloud Native Resource Monitoring Python App on Kubernetes (K8s). It encompasses the use of various technologies and tools such as Python, Flask, Docker, AWS ECR, AWS EKS, and Kubernetes.

## Features
- Monitoring application built with Python using Flask and psutil.
- Dockerized for containerization, enabling easy deployment and scalability.
- Pushes Docker image to AWS ECR for centralized image management.
- Deploys on AWS EKS cluster using Kubernetes for efficient management of resources.

![Cloud_native_monitoring](https://github.com/Rishmish94/Cloud_native_monitoring_project/assets/150320311/fb110573-3fc0-4921-8f45-ccb38b4d6170)


## Prerequisites
Before starting, ensure you have the following installed and configured:
- AWS Account with programmatic access and AWS CLI configured.
- Python3 Installed.
- Docker and Kubectl installed.
- Code editor (e.g., VSCode).

## Getting Started
Follow these steps to set up and run the project:

### Part 1: Deploying the Flask application locally
1. Clone the code repository:
git clone <repository_url>
2. Install dependencies:
pip3 install -r requirements.txt
3. Run the application:
python3 app.py

### Part 2: Dockerizing the Flask application
1. Create a Dockerfile in the root directory of the project.
2. Build the Docker image:
docker build -t <image_name> .
3. Run the Docker container:
docker run -p 5000:5000 <image_name>

### Part 3: Pushing the Docker image to ECR
1. Create an ECR repository using Python and Boto3.
2. Push the Docker image to the ECR repository.

### Part 4: Creating an EKS cluster and deploying the app using Python
1. Create an EKS cluster and node group.
2. Define Kubernetes deployment and service using Python.
3. Run the Python script to deploy the app on Kubernetes.

## Verification and Testing
After deploying the app, verify its status using Kubernetes commands like `kubectl get deployment`, `kubectl get service`, and `kubectl get pods`.

## Acknowledgements
- This project was inspired by the need for a comprehensive resource monitoring solution.
- Special thanks to the developers of Flask, Docker, AWS ECR, AWS EKS, and Kubernetes for their amazing tools and documentation.
