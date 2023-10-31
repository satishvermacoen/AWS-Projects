# 1. Launch an Instance and configure the Web-Server

In this Project, deploy and Configure an EC2 instance as a web server and clone the git repo for the website online.

## AWS Resource Created

1. VPC/subnet
2. EC2 Instance
3. Post config- GIT, Nginx, npm

#### Overview
![Overview]()

### Configuration on AWS Console Portal and Instance Launch.

1. Login to console.
Launch EC2-Instance and fill required configuration for EC2 provision.
![App Screenshot]()

2. Creating a security key pair.
![App Screenshot]()
![App Screenshot]()

3. VPC/Subnet and Public IP for Internet communication.
![App Screenshot]()

4. Launch with default configuration.

![App Screenshot]()

5. Conncet and Login into EC2 Instance through Putty.
![App Screenshot]()

### Post configutration in Insatnce.

6. Configration and installion
- GIT

```bash
    sudo yum install git -y
```
- Nginx

```bash
    sudo yum install nginx -y  
## to start nginx
    sudo systemctl start nginx

```
- npm
```bash
    sudo yum install npm -y 
```
![App Screenshot]()
7. Git Repo cloning in the default path of nginx server. 

```bash
    git clone "https://github.com/satishvermacoen/html/"
```
![App Screenshot]()

8. The website is live, Check throurgh domain name of ec2 instance.
![App Screenshot]()

-------------------------------
Troubleshoot:
- Reboot
- [Stackoverflow](https://stackoverflow.com/questions/49064167/nginx-wont-restart-job-for-nginx-service-failed-because-the-control-proce)
- Some Error Screenshot
![App Screenshot]()
