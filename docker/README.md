# Docker and JupyterLab

Docker was used to deploy the data science environment as an isolated container on the Ubuntu EC2 instance.

## Container Architecture

```text
AWS EC2
   |
Ubuntu Server
   |
Docker Engine
   |
JupyterLab Container
   |
TCP Port 8888
