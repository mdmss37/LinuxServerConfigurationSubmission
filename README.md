# LinuxServerConfigurationSubmission
Repository for Udacity nanodegree submission

#1 The IP address and SSH port so your server can be accessed by the reviewer.
1. IP address is 35.162.154.29
2. Port number as below
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

#2 The complete URL to your hosted web application.
http://ec2-35-162-154-29.us-west-2.compute.amazonaws.com/

#3 A summary of software you installed and configuration changes made.
1. Launch your Virtual Machine with Udacity account
*public IP address is 35.162.154.29
2. Followed the instructions provided to SSH into your server
3. Created a new user named grader
4. Gave the grader the permission to sudo
5. Updated all currently installed packages
6. Changed the SSH port from 22 to 2200
7. Configured the Uncomplicated Firewall (UFW) to only allow incoming connections for SSH (port 2200), HTTP (port 80), and NTP (port 123)
8. Configure the local timezone to UTC
9. Installed and configure Apache to serve a Python mod_wsgi application
10. Installed and configure PostgreSQL
- Do not allow remote connections
- Created a new user named catalog that has limited permissions to your catalog application database
11. Installed git, clone and setup Catalog App project (from GitHub repository from earlier in the Nanodegree program) so that it functions correctly when visiting your server’s IP address in a browser. 
Remember to set this up appropriately so that your .git directory is not publicly accessible via a browser.⋅⋅
-->
Currently App is not correctly served in URL, but showing default apache2 page.
Assuming configuration was wrong, under checking.

#4 A list of any third-party resources you made use of to complete this project.

https://www.digitalocean.com/community/tutorials/how-to-deploy-a-flask-application-on-an-ubuntu-vps
https://discussions.udacity.com/t/markedly-underwhelming-and-potentially-wrong-resource-list-for-p5/8587
https://github.com/elnobun/Linux-Server-Configuration

#5 The thing to do when submission
Open your ~/.ssh/udacity_key.rsa file in a text editor and copy the contents of that file.
During the submission process, paste the contents of the udacity_key.rsa file into the "Notes to Reviewer" field.
