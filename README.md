IEC-RISE-DOCKER-COMPOSE-PROJECT
In this project I have created a blog website using WordPress and MySql. Docker Compose is a tool for defining and running multi-container docker applications. 

Requirements/Installation
These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See deployment for notes on how to deploy the project on a live system.
Make sure you have the latest versions of Docker and Docker Compose installed on your machine.
For installing run the commands:
For Docker Installation on RedHat/Centos:
Configure yum in RedHat/Centos to add Docker for local installation
using "https://download.docker.com/linux/centos/docker-ce.repo" put this link in the file in /etc/yum.repos.d/
 ![1](https://user-images.githubusercontent.com/65006678/82115313-ad28e280-977f-11ea-922e-14d553e2a516.PNG)
![2](https://user-images.githubusercontent.com/65006678/82115613-7eac0700-9781-11ea-95a8-ded7da98c9da.PNG)
 
Now, run command
yum install docker-ce --nobest
Start Docker:
Systemctl enable docker
systemctl start docker

After Docker installation for wordpress and database use below commands:
docker pull wordpress:5.4.1-php.3 apache
docker pull mysql:5.7

![3](https://user-images.githubusercontent.com/65006678/82115614-7fdd3400-9781-11ea-931d-c048283c6c2d.jpg)

![4](https://user-images.githubusercontent.com/65006678/82115615-8075ca80-9781-11ea-8c0b-78f7cbc45808.jpeg)

  iptables –F
Iptables –nvL

 
![5](https://user-images.githubusercontent.com/65006678/82115656-c599fc80-9781-11ea-8377-29210db96543.jpeg)

![6](https://user-images.githubusercontent.com/65006678/82115622-8ff51380-9781-11ea-892a-0a0ef00a8fb4.jpeg)
![7](https://user-images.githubusercontent.com/65006678/82115625-91264080-9781-11ea-9b2a-d6692360f8ac.jpeg)
![8](https://user-images.githubusercontent.com/65006678/82115626-91bed700-9781-11ea-99f4-92de8c5ce0ec.jpeg)
 


 
 
 
install Docker Compose:-
curl -L https://github.com/docker/compose/releases/download/1.21.2/docker-compose-`uname -s`-`uname -m` -o /usr/local/bin/docker-compose
chmod +x /usr/local/bin/docker-compose
After installation of the above files:-

Make a file using
mkdir mycomposet/        (you can give any name)
cd mycompose/

vim docker-compose.yml
(type I as to enter insert mode and :wq after entering esc to save it)
![9](https://user-images.githubusercontent.com/65006678/82115627-92576d80-9781-11ea-89f1-49505ebe4c29.jpeg)
![10](https://user-images.githubusercontent.com/65006678/82115628-92576d80-9781-11ea-8b4c-b8e61f6ee05e.jpeg)
 
 


Go to the project folder in which the .yml file is and run the following command:
docker-compose up -d 
docker-compose up      
 ![11](https://user-images.githubusercontent.com/65006678/82115629-92f00400-9781-11ea-87dd-f573eba18c00.jpeg)

Now open terminal in any new window:
And run:
 ![12](https://user-images.githubusercontent.com/65006678/82115631-93889a80-9781-11ea-8185-d2ded7b704e3.jpeg)


Everything is set now.
 ![13](https://user-images.githubusercontent.com/65006678/82115751-4eb13380-9782-11ea-95b9-8b35a3788bc8.jpeg)
![14](https://user-images.githubusercontent.com/65006678/82115752-507af700-9782-11ea-8f61-ec3142b64073.jpeg)
![15](https://user-images.githubusercontent.com/65006678/82115753-51138d80-9782-11ea-97dc-3b1bf9f16c33.jpeg)
![16](https://user-images.githubusercontent.com/65006678/82115755-51ac2400-9782-11ea-8fa8-18071e52957c.jpeg)


 
 
And to stop the docker compose:
docker-compose stop
Built With
•	RHEL-8 Running in Virtual Box
•	Docker
•	Docker-compose



