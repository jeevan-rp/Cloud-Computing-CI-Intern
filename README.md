☁️ Cloud Computing Tasks – AWS Implementation

This repository contains hands-on implementations of basic cloud computing concepts using AWS, including static website hosting and virtual machine deployment.

📌 TASK 1: Deploy a Static Website on AWS S3
🎯 Objective

To host a static website using AWS S3 Static Website Hosting with public access and a custom error page.

🛠️ Services Used

Amazon S3

AWS Management Console

🔧 Steps Performed

Created an S3 bucket with a globally unique name

Disabled Block Public Access

Uploaded static website files (index.html, error.html)

Enabled Static Website Hosting

Configured Bucket Policy for public read access

Verified website access using S3 website endpoint

📂 Website Files

index.html – Main homepage

error.html – Custom error page

🌐 Output

S3 Website URL:

[http://<bucket-name>.s3-website-<region>.amazonaws.com](http://jeevan-portfolio-aws.s3-website.eu-north-1.amazonaws.com/index.html)

📸 Screenshots (Included)

S3 bucket creation

Uploaded files

Static website hosting enabled

Bucket policy configuration

Website running in browser

Custom error page output

✅ Result

The static website was successfully hosted on AWS S3 and accessed publicly via the S3 website endpoint.

📌 TASK 2: Launch a Virtual Machine (AWS EC2)
🎯 Objective

To launch and configure an AWS EC2 instance, connect via SSH, install a web server, and deploy a webpage.

🛠️ Services Used

Amazon EC2

Amazon Linux 2

Apache HTTP Server (httpd)

🔧 Steps Performed

Launched an EC2 instance (t2.micro) using Amazon Linux 2

Created and used a key pair to connect via SSH

Configured Security Group to allow:

SSH (Port 22)

HTTP (Port 80)

Installed Apache web server

Started and enabled Apache service

Deployed a simple HTML webpage

Accessed webpage using EC2 public IP

🧑‍💻 Commands Used
sudo yum update -y
sudo yum install httpd -y
sudo systemctl start httpd
sudo systemctl enable httpd

🌐 Output

Public IPv4 Address:

http://13.60.49.197/

📸 Screenshots (Included)

EC2 instance running

SSH connection successful

Apache service status (active (running))

Security group inbound rules (HTTP allowed)

Webpage running in browser

✅ Result

The EC2 instance successfully hosted a webpage using the Apache web server and was accessible via its public IP address.

🧠 Key Learnings

Understanding AWS S3 static website hosting

Managing public access using bucket policies

Launching and configuring EC2 instances

Using SSH for remote server access

Installing and running web servers on cloud VMs

Configuring security groups for network access



📎 Note

This repository is created for learning, academic, and demonstration purposes as part of cloud computing practice tasks.
