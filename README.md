Deploy a Python Application on Kubernetes
Overview
In this assignment, you will gain hands-on experience with containerization and orchestration using Docker and Kubernetes. You will deploy a Python web application that displays the current time in Toronto, Canada, using Kubernetes. The application will be containerized using Docker, and you will use NodePort to expose it on port 3030.

Objectives
Create a Dockerfile for the Python application.
Build and push a Docker image to a Docker repository.
Deploy the application on Kubernetes using a Deployment and expose it using a Service of type NodePort.
Document the process and push all necessary files to a GitHub repository.
Steps to Complete the Assignment
Fork and Clone the Repository
Fork the repository containing the Python application: https://github.com/sojoudian/clo835_s24/blob/master/project-2/app.py
Clone your forked repository locally.
Create a Dockerfile
Write a Dockerfile to containerize the Python application. Ensure all dependencies are installed, and the application starts correctly.
Build and Push Docker Image
Build your Docker image using the Dockerfile.
Tag your Docker image and push it to a public Docker repository (e.g., Docker Hub).
Write Kubernetes Manifests
Create a Kubernetes Deployment YAML file to deploy your Docker image.
Create a Kubernetes Service YAML file using NodePort to expose your application on port 3030.
Deploy to Kubernetes
Apply your Kubernetes manifests to deploy your application.
Ensure your Kubernetes cluster is accessible and the application is running correctly.
Test the Application
Access the application via the NodePort and ensure it displays the correct, current time in Toronto/Canada.
Document Your Work
Create a README.md file in your GitHub repository detailing the steps you took, including:
Instructions on how to build and run the Docker container.
Instructions on how to deploy and access the application on Kubernetes.
Document any challenges you faced and how you overcame them.
Submission
Push all your Docker and Kubernetes files, along with your documentation, to your GitHub repository.
Submit a PDF containing:
The URL of your GitHub repository.
A brief description of your project.
Screenshots demonstrating the application running successfully.
Evaluation Criteria
Correctness of the Dockerfile and Kubernetes YAML files.
Functionality of the application when accessed via the exposed NodePort.
Quality and completeness of the documentation in the README.md.
Best practices in Docker usage and Kubernetes configuration.
Resources
Docker Documentation
Kubernetes Documentation
Learn Kubernetes Basics
