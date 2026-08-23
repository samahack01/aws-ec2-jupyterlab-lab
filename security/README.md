# Security

Security for this laboratory was implemented at multiple layers.

## AWS Security Group

The AWS Security Group acted as the network firewall protecting the EC2 instance.

The laboratory required the following inbound services:

- TCP 22 for SSH remote administration.
- TCP 8888 for JupyterLab web access.

If TCP port 8888 were not allowed by the Security Group, external clients would not be able to reach the JupyterLab service even if the Docker container were running correctly.

## SSH Authentication

Remote administration was performed through SSH using an AWS key pair.

The private `.pem` key is intentionally excluded from this public repository.

## System Updates

The Ubuntu server was updated before additional services were installed.

Keeping the operating system and packages updated reduces exposure to known vulnerabilities and improves software compatibility.

## Public Repository Policy

The following information is intentionally excluded from this repository:

- AWS private keys
- Passwords
- Jupyter authentication tokens
- AWS credentials
- Active public IP addresses

Only documentation, architecture, and non-sensitive technical evidence are published.
