# docker-resume-project
Containerized a static resume website using Docker and deployed it on an Amazon Web Services EC2 instance using Apache HTTP server.

## Project Overview
This project demonstrates how to containerize and deploy a static resume website using Docker.  The website is hosted with Apache HTTP Serverand deployed on an Amazon Web Services EC2 instance.

## Tools & Technologies
- Docker
- Apache HTTP Server
- Docker Hub
- Amazon Web Services EC2
- Linux

## Dockerfile
From httpd:latest
Copy ./user/local/apache2/htdocs/

## Steps to Run the Projcet
# 1. Build Docker Imag
 docker build -t ramesh_resume
# 2. Run docker Container
   docker run -d -p 80:80 ramesh_resume
# 3. Tag Docker Image
 docker tag ramesh_resume ramesh55kumar/ramesh_resume:v1.0
# 4. Push Image to Docker Hub
 docker push ramesh55kumar/ramesh_resume:v1.0
 ## Access the Website 
 http://13.126.205.13
   
