# 🚀 VProfile Phase 01 – Manual Deployment & Infrastructure Automation with Vagrant

## 📌 Overview

This repository demonstrates the first phase of my **VProfile DevOps Learning Journey**, where I deployed a production-style multi-tier Java application by first performing a complete manual deployment and then automating the infrastructure using **Vagrant**.

The primary objective of this project was to understand how enterprise applications are deployed, configured, and managed before moving on to advanced DevOps practices such as cloud deployment, CI/CD, containerization, Kubernetes, Infrastructure as Code, and DevSecOps.

---

# 🎯 Objectives

* Understand the architecture of a production-style multi-tier application.
* Deploy each infrastructure component manually.
* Gain hands-on Linux system administration experience.
* Configure communication between multiple servers.
* Learn Infrastructure as Code (IaC) concepts using Vagrant.
* Build a reproducible local development environment.

---

# 🏗️ System Architecture

```text
                    Client
                       │
                       ▼
                 Nginx (Web Tier)
                       │
                       ▼
              Apache Tomcat
            (Java Web Application)
            ┌──────────┼──────────┐
            ▼          ▼          ▼
       MySQL      Memcached    RabbitMQ
      Database      Cache      Messaging
```

The application is distributed across **five virtual machines**, simulating a production-like environment.

| Virtual Machine | Component     | Purpose                    |
| --------------- | ------------- | -------------------------- |
| VM 1            | Nginx         | Reverse Proxy & Web Server |
| VM 2            | Apache Tomcat | Java Application Server    |
| VM 3            | MySQL         | Relational Database        |
| VM 4            | Memcached     | In-Memory Caching          |
| VM 5            | RabbitMQ      | Message Broker             |

---

# 🛠️ Technologies Used

### Operating System

* Linux

### Virtualization

* Vagrant
* VirtualBox

### Web Layer

* Nginx

### Application Layer

* Apache Tomcat
* Java
* Maven

### Database

* MySQL

### Caching

* Memcached

### Messaging

* RabbitMQ

---

# 📖 Project Phases

## Phase 1 – Manual Deployment

Every server was configured manually to gain a deep understanding of production environments.

Activities included:

* Installing required software packages
* Configuring Linux servers
* Setting up networking
* Configuring Nginx
* Deploying the Java application to Tomcat
* Installing and configuring MySQL
* Configuring Memcached
* Configuring RabbitMQ
* Verifying communication between all services

This phase provided practical experience with Linux administration, service management, networking, and application deployment.

---

## Phase 2 – Infrastructure Automation

After successfully completing the manual deployment, the infrastructure was automated using **Vagrant**.

Using a single command:

```bash
vagrant up
```

the project provisions:

* Five virtual machines
* Network configuration
* Service installation
* Infrastructure initialization

This demonstrates the principles of **Infrastructure as Code (IaC)** and enables consistent, repeatable deployments.

---

# 📚 Key Concepts Learned

* Multi-tier Architecture
* Linux System Administration
* Virtualization
* Infrastructure as Code
* Server Provisioning
* Network Configuration
* Reverse Proxy Configuration
* Java Application Deployment
* Service Management
* Production Environment Design

---

# 🎯 Skills Demonstrated

* Linux Administration
* Infrastructure Provisioning
* Virtual Machine Management
* Nginx Configuration
* Apache Tomcat Administration
* MySQL Configuration
* Memcached Configuration
* RabbitMQ Administration
* Infrastructure Automation
* Production Architecture Fundamentals

---

# 🚀 Learning Outcome

This project established the foundation of my DevOps journey by helping me understand how production-grade applications are deployed and managed across multiple servers.

Rather than relying solely on automation tools, I first learned how each component works individually before automating the environment with Infrastructure as Code. This approach strengthened my understanding of enterprise infrastructure and prepared me for more advanced topics such as cloud computing, CI/CD, Docker, Kubernetes, Terraform, Ansible, and DevSecOps.

---

# 🛣️ Roadmap

This repository is the first milestone in my VProfile learning journey.

Upcoming phases include:

* AWS Deployment
* Jenkins CI/CD
* GitHub Actions CI/CD
* GitLab CI/CD
* Docker
* Kubernetes
* Terraform
* Ansible
* DevSecOps Pipeline

---

# 📄 License

This repository is created for educational purposes to demonstrate DevOps concepts, infrastructure automation, and production-style deployment practices.
