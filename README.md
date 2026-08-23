# AWS EC2 JupyterLab Lab

Cloud infrastructure laboratory focused on deploying a containerized data science environment on Amazon Web Services.

The project demonstrates the provisioning of an Ubuntu Server EC2 instance, secure remote administration through SSH, Docker-based application deployment, AWS Security Group configuration, and JupyterLab service exposure through TCP port 8888.

## Architecture

The environment follows this logical flow:

```text
Local Laptop
PowerShell + SSH
      |
      | TCP 22
      v
AWS Security Group
      |
      v
AWS EC2
Ubuntu Server
      |
      v
Docker
      |
      v
JupyterLab
      |
      | TCP 8888
      v
Internet / Web Client
