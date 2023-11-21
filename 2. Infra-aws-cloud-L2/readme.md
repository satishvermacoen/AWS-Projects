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


### Configuration on AWS Console Portal and Instance Launch.

1. Login to console.
Launch EC2-Instance and fill required configuration for EC2 provision.
![App Screenshot]()

2. To launch 3 instance with use of bash script without public-ip

```bash 
aws ec2 run-instances --image-id ami-02a2af70a66af6dfb --count 3 --instance-type t2.micro --key-name ansiblekey --security-group-ids sg-0dae92cc1189d04c4 --subnet-id subnet-02d5bfa67e716132f


```

3. To Documentation of ansible page link -
 https://docs.ansible.com/ansible/latest/installation_guide/installation_distros.html#installing-ansible-on-ubuntu 


4. To Installing Ansible on Ubuntu.

```bash
sudo apt update -y

sudo apt install software-properties-common -y

sudo add-apt-repository --yes --update ppa:ansible/ansible

sudo apt install ansible -y

```