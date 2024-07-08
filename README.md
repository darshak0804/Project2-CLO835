<<<<<<< HEAD
There are some of the steps we need to do to complete this assignment.

Step 1:

First of all, we need to fork or clone the git repository which have app.py in our case professor gave us the python file to complete this project.

After getting the python file I cloned that in my local machine.

Step 2:

In the second task we need to create Dockerfile in root folder with the content of working directory, necessary dependencies and on which port application will run.

Meanwhile just push the Dockerfile to github.

Step 3:

In this step, we need to build the docker image 

Firstly login to docker hub and then create the image

Docker build –t darshak0804/project2clo835 .
 
And push the image to docker hub 

Docker push darshak0804/projectclo835:latest

Step 4:
  
Manifesting Kubernetes files like “deployment.yaml” and “service.yaml”

•	Creating a Kubernetes Deployment YAML file to deploy my Docker image “project2clo835”.

And 

Creating a Kubernetes Service YAML file using NodePort to expose my application on port 3030.

Step 5:

Deploying application through manifesting kubernetes.

Make sure your minikube is start if it’s not then run below command to start and check status:

Minikube start
 
Minikube status

Then 

Apply the deployment and service manifests

Kubectl apply –f deployment.yaml
Kubectl apply –f service.yaml



Check the status of my deployment 

Kubectl get deployments

Kubectl get pods

Kubectl get services

Step 6:

To Test the Application access using the NodePort. Finding the external IP of Kubernetes node 

In my case 

http://172.23.239.167:30300 to access the application and the the output of current location and time
=======
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
>>>>>>> 1471794d66c03dff6efd1977addc45762fb2566d
