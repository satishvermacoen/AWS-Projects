# 1. Launch an Instance and configure the Web-Server

In this Project, deploy and Configure an EC2 instance as a web server and clone the git repo for the website online.

## AWS Resource Created

1. VPC/subnet
2. EC2 Instance
3. Post config- GIT, Nginx, npm

#### Overview
![Overview](https://github.com/satishvermacoen/AWS-Projects/blob/main/1.%20Launch%20an%20Instance%20and%20configure%20Web-Server/img/overview.png)

### Configuration on AWS Console Portal and Instance Launch.

1. Login to console.
Launch EC2-Instance and fill required configuration for EC2 provision.
![App Screenshot](https://github.com/satishvermacoen/AWS-Projects/blob/main/1.%20Launch%20an%20Instance%20and%20configure%20Web-Server/img/Screenshot%20(86).png)

2. Creating a security key pair.
![App Screenshot](https://github.com/satishvermacoen/AWS-Projects/blob/main/1.%20Launch%20an%20Instance%20and%20configure%20Web-Server/img/Screenshot%20(87).png)

3. VPC/Subnet and Public IP for Internet communication.
![App Screenshot](https://github.com/satishvermacoen/AWS-Projects/blob/main/1.%20Launch%20an%20Instance%20and%20configure%20Web-Server/img/Screenshot%20(90).png)

4. Launch with default configuration.

![App Screenshot](https://github.com/satishvermacoen/AWS-Projects/blob/main/1.%20Launch%20an%20Instance%20and%20configure%20Web-Server/img/Screenshot%20(92).png)

![App Screenshot](https://github.com/satishvermacoen/AWS-Projects/blob/main/1.%20Launch%20an%20Instance%20and%20configure%20Web-Server/img/Screenshot%20(84).png)
5. Conncet and Login into EC2 Instance through Putty.
![App Screenshot](https://github.com/satishvermacoen/AWS-Projects/blob/main/1.%20Launch%20an%20Instance%20and%20configure%20Web-Server/img/Screenshot%20(97).png)

![App Screenshot](https://github.com/satishvermacoen/AWS-Projects/blob/main/1.%20Launch%20an%20Instance%20and%20configure%20Web-Server/img/Screenshot%20(98).png)

### Post configutration in Insatnce.

6. Configration and installion
- GIT

```bash
    sudo yum install git -y
```
![App Screenshot](https://github.com/satishvermacoen/AWS-Projects/blob/main/1.%20Launch%20an%20Instance%20and%20configure%20Web-Server/img/Screenshot%20(99).png)

- npm
```bash
    sudo yum install npm -y 
```

- Nginx

```bash
    sudo yum install nginx -y  
## to start nginx
    sudo systemctl start nginx
```
![App Screenshot](https://github.com/satishvermacoen/AWS-Projects/blob/main/1.%20Launch%20an%20Instance%20and%20configure%20Web-Server/img/Screenshot%20(100).png)


7. Git Repo cloning in the default path of nginx server. 

```bash
## Default Path
    cd /usr/share/nginx/html

    git clone "https://github.com/satishvermacoen/html/"

```
![App Screenshot](https://github.com/satishvermacoen/AWS-Projects/blob/main/1.%20Launch%20an%20Instance%20and%20configure%20Web-Server/img/Screenshot%20(105).png)

8. The website is live, Check throurgh domain name of ec2 instance.
![App Screenshot](https://github.com/satishvermacoen/AWS-Projects/blob/main/1.%20Launch%20an%20Instance%20and%20configure%20Web-Server/img/Screenshot%20(106).png)

-------------------------------
Troubleshoot:
- Reboot
- [Stackoverflow](https://stackoverflow.com/questions/49064167/nginx-wont-restart-job-for-nginx-service-failed-because-the-control-proce)
- Some Error Screenshot
![App Screenshot](https://github.com/satishvermacoen/AWS-Projects/blob/main/1.%20Launch%20an%20Instance%20and%20configure%20Web-Server/img/Screenshot%20(101).png)
![App Screenshot](https://github.com/satishvermacoen/AWS-Projects/blob/main/1.%20Launch%20an%20Instance%20and%20configure%20Web-Server/img/Screenshot%20(102).png)
![App Screenshot](https://github.com/satishvermacoen/AWS-Projects/blob/main/1.%20Launch%20an%20Instance%20and%20configure%20Web-Server/img/Screenshot%20(103).png)
![App Screenshot](https://github.com/satishvermacoen/AWS-Projects/blob/main/1.%20Launch%20an%20Instance%20and%20configure%20Web-Server/img/Screenshot%20(104).png)
