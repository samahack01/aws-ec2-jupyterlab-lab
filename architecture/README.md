# Architecture

This section documents the logical architecture of the AWS EC2 JupyterLab environment.

The environment combines remote administration through SSH with a containerized JupyterLab service hosted on an Ubuntu Server EC2 instance.

## Network Flow

- The local workstation connects to the EC2 instance through SSH using TCP port 22.
- Ubuntu Server runs as the operating system of the EC2 instance.
- Docker provides the container runtime.
- JupyterLab runs inside the Docker environment.
- TCP port 8888 provides web access to the JupyterLab service.
- AWS Security Groups control inbound network access to the instance.
