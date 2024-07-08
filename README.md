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
