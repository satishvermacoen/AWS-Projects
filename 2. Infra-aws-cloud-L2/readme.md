# 2. Infra Deployment on AWS

In this Project, deploy and Configure an 2-EC2 instance as a web server and using Elastic Load Balancing, AWS WAF, Route-53, Public & Private Subnet.

### AWS Resource Created

1. VPC/subnet
2. EC2 Instance
3. Elastic Load Balancing 
4. AWS WAF 
5. Route-53
6. Public & Private Subnet
7. Post config- GIT, Nginx, npm
8. Domain - satishverma.cloud

![Overview](https://github.com/satishvermacoen/AWS-Projects/blob/main/2.%20Infra-aws-cloud-L2/img/2.%20awsinfra.png)

### Configuration on AWS Console Portal and Instance Launch.

1. Login to console.
Launch EC2-Instance and fill required configuration for EC2 provision.
![App Screenshot]()

2. To launch 2 instance with use of bash script without public-ip

```bash 
aws ec2 run-instances --image-id ami-02a2af70a66af6dfb --count 2 --instance-type t2.micro --key-name nginxkey --security-group-ids sg-0dae92cc1189d04c4 --subnet-id subnet-02d5bfa67e716132f


```

3. To Documentation of nginx page link -
 

4. To Installing nginx on Ubuntu.

```bash
sudo apt-get update -y

sudo apt-get install nginx -y

```