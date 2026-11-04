# AWS IAM & EC2 – Web Server Deployment

## Codomax Cloud & DevOps Internship | Module 02

### Project Overview

This project demonstrates how to launch, configure, and secure an Amazon EC2 instance and deploy a basic HTML website using Apache Web Server.

It was developed as part of Module 02 of the Codomax AWS Cloud & DevOps Virtual Internship.

### Technologies Used

- **Amazon EC2** – Cloud-based virtual server
- **Amazon Linux 2023** – Server operating system
- **Apache HTTP Server** – Website hosting
- **AWS IAM** – Identity and access management fundamentals
- **AWS Security Groups** – Network access control
- **HTML and CSS** – Website development
- **GitHub** – Source code and documentation

### EC2 Configuration

| Component | Configuration |
|---|---|
| Instance type | t3.micro |
| Operating system | Amazon Linux 2023 |
| AWS Region | Asia Pacific (Sydney) – ap-southeast-2 |
| Storage | 8 GiB gp3 |
| Web server | Apache HTTP Server |
| HTTP port | 80 |
| SSH port | 22 (restricted access) |

### Deployment Steps

1. Explored IAM roles, policies, users, and least-privilege access principles.
2. Launched an Amazon EC2 instance using Amazon Linux 2023.
3. Configured a Security Group with public HTTP access and restricted SSH access.
4. Connected to the EC2 instance using EC2 Instance Connect.
5. Installed Apache HTTP Server.
6. Started and enabled the Apache service.
7. Created an `index.html` file in `/var/www/html/`.
8. Accessed the deployed website through the EC2 public IPv4 address.

### Apache Installation Commands

```bash
sudo dnf update -y
sudo dnf install httpd -y
sudo systemctl start httpd
sudo systemctl enable httpd
sudo systemctl status httpd
```

### Live Website

http://13.239.116.188

*Note: This is a temporary EC2 public IP address. The website may become unavailable when the instance is stopped or terminated.*

### Security Practices

- Used IAM concepts to understand access permissions and least privilege.
- Restricted SSH access through Security Group rules.
- Allowed HTTP traffic on port 80 for public website access.
- Kept the private SSH key outside the public GitHub repository.
- Used a small Free Tier-eligible EC2 instance to minimize cloud costs.

### Learning Outcomes

Through this project, I learned how to:

- Understand basic AWS IAM concepts.
- Launch and configure an EC2 instance.
- Configure inbound Security Group rules.
- Connect to a Linux cloud server.
- Install and manage Apache.
- Deploy a basic HTML website to AWS.
- Understand basic cloud security and cost management.

### Conclusion

This module provided practical experience with AWS compute services, Linux server administration, web hosting, and basic cloud security. It establishes a foundation for future modules involving Amazon S3, VPC, RDS, serverless computing, and CI/CD.

---

**Codomax Digital Solutions – AWS Cloud & DevOps Virtual Internship 2026**
