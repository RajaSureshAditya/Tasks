Docker
------
Task 1
======
Write a Dockerfile (CentOS 6) to install the following in a Docker container:

Python 2.7

MongoDB - any version

Apache tomcat 7 - running on port 8080

Please include comments at every command explaining what it does.

Write the command to run the Dockerfile such that once the container boots, apache tomcat's home page is accessible from the host on port 7080.
Pre-requisites
--------------
Docker 1.3 >


Docker container with 7080 port on host and 8080 on container

for building the docker image run the command where you have Dockerfile 

docker build -t tomcat7 .

To get your Application in the container running run the below command 

docker run -it --name tomcat7 -p 7080:8080 -p 27017:27017 tomcat7


Here -i is for interactive and t is for terminal



