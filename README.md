# Docker11

Project-1

Docker IMAGE of my WebServices
This Project will allow you to migrate that WebService into a docker container instance, that acts as a more portable and modular framework for hosting services.<br>
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
6.	Check in the browser with your instance ip(ip:8081/).<br>
