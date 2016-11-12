# LinuxServerConfigurationSubmission
Repository for Udacity nanodegree

1. The IP address and SSH port so your server can be accessed by the reviewer.
IP address is 35.162.154.29
#Port number
```
grader@ip-10-20-63-124:~$ sudo ufw status
Status: active

To                         Action      From
--                         ------      ----
2200/tcp                   ALLOW       Anywhere
80/tcp                     ALLOW       Anywhere
123/udp                    ALLOW       Anywhere
2200/tcp (v6)              ALLOW       Anywhere (v6)
80/tcp (v6)                ALLOW       Anywhere (v6)
123/udp (v6)               ALLOW       Anywhere (v6)
```
2. The complete URL to your hosted web application.
http://ec2-35-162-154-29.us-west-2.compute.amazonaws.com/

3. A summary of software you installed and configuration changes made.
Launch your Virtual Machine with Udacity account.
Follow the instructions provided to SSH into your server
Create a new user named grader
Give the grader the permission to sudo
Update all currently installed packages
Change the SSH port from 22 to 2200
Configure the Uncomplicated Firewall (UFW) to only allow incoming connections for SSH (port 2200), HTTP (port 80), and NTP (port 123)
Configure the local timezone to UTC
Install and configure Apache to serve a Python mod_wsgi application
Install and configure PostgreSQL:
Do not allow remote connections
Create a new user named catalog that has limited permissions to your catalog application database
4. A list of any third-party resources you made use of to complete this project.

https://www.digitalocean.com/community/tutorials/how-to-deploy-a-flask-application-on-an-ubuntu-vps
https://discussions.udacity.com/t/markedly-underwhelming-and-potentially-wrong-resource-list-for-p5/8587
https://github.com/elnobun/Linux-Server-Configuration

Open your ~/.ssh/udacity_key.rsa file in a text editor and copy the contents of that file.
During the submission process, paste the contents of the udacity_key.rsa file into the "Notes to Reviewer" field.
