---
title: "Cloud Infrastructure"
author: "Brandon Clark"
description: "A summary of what I've learned this semester for the topic of cloud infrastructure."
published: "2024-2-14"
---
# Cloud Infrastructure
## EC2
Search for EC2 on AWS; launching an instance on EC2 takes:
#### An operating system (RedHat Linux)
- The operating system is what the computer will be running.
#### An instance type (t2.micro)
- The instance type is the hardware that AWS will be using.
#### A security key pair
- The security key pair file will allow access through the PuTTY terminal.
#### A security group
- The security group will allow computers to communicate on certain ports.

### Use the security pair, the public IPv4 address, and connect using the PuTTY terminal.

After connecting, install a web server:
```sh
sudo yum install httpd
```
Then start the web server:
```sh
sudo systemctl start httpd
```

## S3
Search for S3 on AWS.
- Name the S3 bucket
- Allow all public access and check the box to acknowledge the risks
![Allowing public access](/images/devopsfinal2.png)
- Enable bucket versioning
![Enabled bucket versioning](/images/devopsfinal1.png)

Finish and create the bucket.