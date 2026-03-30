# Standard Operating Procedure (SOP)  
## Setup of Virtual Linux Server for Web Application Testing  

**Student Name:** Angadveer singh  
**Course:** NSA  
**Instructor:** Felix  
**Date:** March 30, 2026  

---

## Purpose
The purpose of this SOP is to provide clear and simple steps to set up a virtual Linux server for web application testing. The expected outcome is a fully working server with Apache, MySQL, and PHP installed and ready for testing.

---

## Scope
This SOP applies to students and IT staff who need to create a Linux-based virtual machine for testing purposes.

Objectives:
- Create a virtual machine  
- Install Ubuntu Server  
- Configure system settings  
- Install required software packages  
- Test the web server  

---

## Accountability Matrix

| Task | Responsible |
|------|------------|
| VM Creation | System Administrator |
| OS Installation | System Administrator |
| Software Installation | DevOps |
| Testing | QA Tester |
| Documentation | IT Support |

---

## Reversion Info

| Version | Date | Changes |
|--------|------|--------|
| 1.0 | 2026-03-30 | Initial version created |
| 1.1 | 2026-03-30 | Added testing and verification steps |

---

## Approval Table

| Name | Role | Signature | Date |
|------|------|----------|------|
| Student | Author | ______ | 2026-03-30 |
| Instructor | Reviewer | ______ | ______ |

---

## Definitions
- **VM:** Virtual Machine  
- **Linux:** Operating system used for servers  
- **Apache:** Web server software  
- **MySQL:** Database system  
- **PHP:** Server-side scripting language  

---

## Procedure Steps

### Step 1: Create Virtual Machine
- Open VirtualBox or VMware  
- Click on “New”  
- Select Linux → Ubuntu (64-bit)  
- Allocate 4 GB RAM and 2 CPU cores  
- Attach Ubuntu ISO file  

---

### Step 2: Install Linux OS
- Start the virtual machine  
- Select language and keyboard  
- Set hostname (webtest-server)  
- Create username and password  
- Complete installation  

---

### Step 3: Update System
```bash
sudo apt update
sudo apt upgrade -y
Step 4: Install Required Software
sudo apt install apache2 -y
sudo apt install mysql-server -y
sudo apt install php libapache2-mod-php php-mysql -y
Step 5: Test Web Server
Open browser
Enter server IP address
Verify Apache default page

Create test file:

cd /var/www/html
sudo nano index.php

Add:

<?php phpinfo(); ?>
Save and refresh browser
Reference or Related Documents
Ubuntu Official Documentation
Apache Documentation
MySQL Documentation
VMware / VirtualBox Guide
Conclusion

This SOP provides a simple and structured process to set up a virtual Linux server for web application testing. Following these steps ensures a stable and properly configured testing environment.
