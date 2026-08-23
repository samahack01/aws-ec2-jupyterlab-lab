# Deployment

This section documents the main deployment workflow used to build the AWS-hosted JupyterLab environment.

## EC2 Provisioning

An Ubuntu Server instance was provisioned using Amazon EC2.

The instance provided the cloud computing environment used to host Docker and the JupyterLab service.

## Remote Administration

The EC2 instance was accessed remotely from a Windows workstation using PowerShell and SSH.

```bash
ssh -i private-key.pem ubuntu@EC2_PUBLIC_IP
