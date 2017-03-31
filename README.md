# Docker11

Project-1

Docker IMAGE of my WebServices:
Docker is a technology that allows us to build, run, test, and deploy distributed applications that are based on Linux containers. 

This  project is used to install our hw2 and hw3 into our docker application using GIT and Dockerfile.
This Project will allow us to migrate that WebService into a docker container instance, that acts as a more portable and modular framework for hosting services.<br>
##STEPS TO RUN THE IMAGE: 
<b>DOWNLOAD THE IMAGE FROM THE URL</b>
https://drive.google.com/open?id=0B0-vnQi5a-hJOXRpajlUdkVnSlU

<br>
1.	Install the docker in aws environment.<br> 
Install (as root): yum install docker-io <br>
Start the docker service (as root): service docker start<br>
2.	Docker load -i output.tar<br>
3.	//new image will be created and displays the image-id.<br>
4.	Copy the newly created image0id(visible below the docker load command).<br>
5.	Docker run -d -p 8081:80 <copied id> <br>
6.	Check in the browser with your instance ip(ip:8077/).<br>



Steps followed in order to build the docker for my application:

1) Launched an Linux instance and login as sudo su administrator.

2)Install docker using below step:
    yum install docker-io
	
	
3)Start docker using below steps:
  service docker start
	
4)Install git in the instance using below step:
  yum install git
  
  
5)Cloned my git project url as follows:
git clone https://github.uc.edu/suggusi/Docker11

6)cat Dockerfile

7)To build the docker image from the docker file:
docker build -t webserver

8)Run docker images to verify that the image was created correctly and that the image name contains a repository that I pushed.ie.web server
    docker images
	
9)docker run -p 80:80 webserver

10)To create container for the image by running it:
docker run -it -d keerthi/webserver

11)To check the container-id:
 docker ps -a
 
12)To execute:
docker exec -it <containerid>  bash

13)To have the listener port :80 inside the docker container:
apt-get update

14)apt-get install vim

15)cd conf

16)vi server.xml

17)cd webapps

18)rm -r ROOT

19)mv CloudAssign2 ROOT

20)exit

21)To commit the docker:
docker commit <container-id>  newwebserver:final

22)To save docker images and create .tar file
docker save <image-id> > output.tar


23)This is uploaded in my google drive which is below:
https://drive.google.com/open?id=0B0-vnQi5a-hJOXRpajlUdkVnSlU
