Jenkins CI/CD Pipeline with Docker

Objective:

Set up a basic Jenkins pipeline to automate the process of building and deploying a simple Node.js application using Docker.

Tools Used

- Jenkins
- Docker
- Git bash



 Jenkinsfile (Pipeline Script)

The 'Jenkinsfile' defines a simple CI/CD pipeline with the following stages:

1. Launching the EC2 instance
2.Install Packages like Docker and Jenkins container
3.Access this container using 8080 port number 
4.Create a new Jenkins jobs and run pipeline script to build ,test and deploy

 
Commands:
1.Sudo apt update 
2.sudo apt install docker.io -y
3.sudo docker run --name c1 -d -p 7070:8080 Jenkins/Jenkins
4.sudo docker exec -u root -it c1 bash
