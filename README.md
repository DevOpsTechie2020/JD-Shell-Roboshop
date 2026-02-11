![roboshop](https://github.com/user-attachments/assets/5c9152c6-153c-4190-8cfd-5ae8919d8268)


**3-Tier Architeccture Deployment on AWS using Shell Scripting**

Project Overview

This project demonstrates a fully automated deployment of a 3 tier architecture e commerce application on AWS using EC2 instances and shell scripting automation.All infrastructure components,DNS configuration and instance provisioning were automated using **bash scripting**** without using Infrastructure as Code tools like Terraform or Cloudformation.

The architecture follows a standard 3-tier model:

1.Frontend Tier

2.Backend (Application/Microservices) Tier

3.Database Tier

Each component runs on dedicated EC2 instances and communicates internally using private IP addresses and sub-domains assigned to them.

**Architecture Design**
    
    **1.Frontend**
        Nginx web server which serves as UI and communicates with backend APIs
    
    **2.Backend**
        
        Catalouge
        
        User
        
        Cart
        
        Shipping
        
        Payment

    **3.Database**

        MongoDB

        MySQL

        Redis

        RabbitMQ

**Infrastructure Automation**

Everything is automated using Bash Shell Scripting:

Instances launched using AWS CLI with automated tagging and naming

Route53 is configured manually in AWS console and custom domain integration and name servers updated.

Subdomains are created automatically for each service using script and mapped to private IP address

**Instance Configuration**

Each instance is automatically configured with 

    --> Requuired Package Installation

    --> Application Deployment

    --> Service configuration

    --> Dependency setup

    --> Service startup and enablement

**Key Highlights**

Fully automated infrastructure provisioning by running bash scripts for each instance

Zero Manual configuration

Real world 3-tiet deployment model

**Future Improvements**

Convert shell scripts to terraform

Add CI/CD pipeline like GitHUb actions and Jenkins

Implement load balancer and Autoscaling

This project showcases hands on DevOps skills including infrastructure automation, DNS management and distributed application deployment in AWS.
