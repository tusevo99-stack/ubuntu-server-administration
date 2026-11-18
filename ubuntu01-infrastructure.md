# Ubuntu01 — AWS Infrastructure Documentation

## 1. Overview

Ubuntu01 is a Linux web server deployed on Amazon Web Services (AWS). It provides a practical environment for learning and documenting cloud infrastructure, Linux system administration, and web hosting.

## 2. Operating System

- Distribution: Ubuntu Server 24.04.5 LTS
- Codename: Noble
- Kernel: Linux 7.0.0-1014-aws
- Architecture: x86_64

## 3. Hardware Resources

- CPU: 2 virtual CPUs
- Processor: Intel Xeon Platinum 8259CL
- Memory: approximately 909 MiB
- Swap: 1 GiB
- Root filesystem: approximately 6.8 GB

These values represent a snapshot of the server configuration and resource availability during inspection.

## 4. Web Hosting Stack

| Component | Version |
|---|---|
| Apache | 2.4.58 |
| PHP | 8.3.6 |
| MariaDB | 10.11.14 |

### Apache Configuration

- MPM: prefork
- PHP integration: mod_php
- Service status: active and running

### PHP Extensions

- mysqli
- mysqlnd
- PDO MySQL
- cURL
- GD
- mbstring
- XML
- ZIP
- OPcache

### Database

MariaDB is installed and its service is active.

## 5. Cloud Environment

- Cloud provider: Amazon Web Services
- Compute service: Amazon EC2
- Operating system: Ubuntu Server

## 6. Administration and Monitoring

The following Linux commands were used to inspect the server:

- `lsb_release -a` — operating system information
- `uname -a` — kernel information
- `free -h` — memory and swap usage
- `df -h` — filesystem usage
- `lscpu` — CPU information
- `apache2 -v` — Apache version
- `php -v` — PHP version
- `mariadb --version` — MariaDB version
- `systemctl status apache2` — Apache service status

## 7. Security

Sensitive information such as private IP addresses, public IP addresses, SSH keys, passwords, access tokens, and customer data is intentionally excluded from this repository.

## 8. Project Goals

- Document practical AWS and Linux administration.
- Improve cloud infrastructure management skills.
- Explore server monitoring and resource optimization.
- Develop automation scripts.
- Contribute to open-source projects.

## 9. Author

Samuel Tusevo  
GitHub: https://github.com/tusevo99-stack  
Organization: TuseGlobTech

## 10. Project Status

Ongoing technical documentation and infrastructure learning project.

---

## 11. Infrastructure Architecture

The Ubuntu01 server is deployed on Amazon Web Services (AWS) using the EC2 compute service.

### Architecture Components

1. Internet — External access to hosted services.
2. DNS — Domain name resolution.
3. AWS EC2 — Virtual machine hosting the server.
4. Ubuntu Server 24.04 LTS — Operating system.
5. Apache — Web server.
6. PHP — Application runtime.
7. MariaDB — Relational database management system.

### Technology Stack

- Cloud Platform: Amazon Web Services
- Compute: Amazon EC2
- Operating System: Ubuntu Server
- Web Server: Apache
- Backend: PHP
- Database: MariaDB

### Architecture Overview

Internet → DNS → AWS EC2 → Ubuntu Server → Apache → PHP → MariaDB

This architecture represents the main components of the Ubuntu01 web hosting environment.
