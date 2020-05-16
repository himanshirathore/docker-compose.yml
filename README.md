IEC-RISE-DOCKER-COMPOSE-PROJECT
In this project I have created a blog website using WordPress and MySql. Docker Compose is a tool for defining and running multi-container docker applications. 

Requirements/Installation
These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See deployment for notes on how to deploy the project on a live system.
Make sure you have the latest versions of Docker and Docker Compose installed on your machine.
For installing run the commands:
For Docker Installation on RedHat/Centos:
Configure yum in RedHat/Centos to add Docker for local installation
using "https://download.docker.com/linux/centos/docker-ce.repo" put this link in the file in /etc/yum.repos.d/
 
 
Now, run command
yum install docker-ce --nobest
Start Docker:
Systemctl enable docker
systemctl start docker

After Docker installation for wordpress and database use below commands:
docker pull wordpress:5.4.1-php.3 apache
docker pull mysql:5.7
  iptables –F
Iptables –nvL

 

 


 
 
 
install Docker Compose:-
curl -L https://github.com/docker/compose/releases/download/1.21.2/docker-compose-`uname -s`-`uname -m` -o /usr/local/bin/docker-compose
chmod +x /usr/local/bin/docker-compose
After installation of the above files:-

Make a file using
mkdir mycomposet/        (you can give any name)
cd mycompose/

vim docker-compose.yml
(type I as to enter insert mode and :wq after entering esc to save it)
systemctl restart docker
 
 


Go to the project folder in which the .yml file is and run the following command:
docker-compose up -d    (for rumming in background)
docker-compose up       (to see the activities)
 

Now open terminal in any new window:
And run:
 


Everything is set now.
 

 
 
And to stop the docker compose:
docker-compose stop
Built With
•	RHEL-8 Running in Virtual Box
•	Docker
•	Docker-compose
•	Docker images:
o	Mysql
Wordpress

