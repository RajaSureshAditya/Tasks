Docker
------

Docker container with 7081 port on host and 8080 on container

for building the docker image run the command where you have Dockerfile 

docker build -t tomcat7 .

To get your Application in the container running run the below command 

docker run -it --name tomcat7 -p 7081:8080 -p 27017:27017 tomcat7


Here -i is for interactive and t is for terminal



