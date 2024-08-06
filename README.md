# Application-Deployment-Using-Docker-Containers
This project demonstrates the deployment of a two-tier application using Docker. The application consists of a Flask web application container and a MySQL database container. Docker Compose is used to manage and orchestrate the deployment of these containers.

Tech Involved-
Python Webapp
Docker
MySql Database
MySql Workbench

Essential Commands-
1. To build an image
   docker build -t <image-name> .
2. To view all images
   docker images
3. To create common network to establish a connection between two containers
   docker create network <name of the network>
4. To run the image
   docker run --network test -p 5001:5000 <image-name>

5. To run dockercompose file
   docker-compose -f <name.yaml> up

MySQL Database Queries - 
 CREATE DATABASE flaskapp;
 show databases;
 USE flaskapp;
 CREATE TABLE users(name varchar(20),email varchar(40));
 SELECT * from users;
 ALTER USER 'root'@'%' IDENTIFIED WITH mysql_native_password BY 'my-secret-pw'; FLUSH PRIVILEGES;


