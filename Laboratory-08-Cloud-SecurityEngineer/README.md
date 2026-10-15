# Laboratory 08: The Cloud Security Engineer

## Mission Overview

This laboratory activity focuses on securing an Ubuntu server using UFW (Uncomplicated Firewall). It involves deploying a web application, checking network ports, and configuring firewall rules to allow only the required traffic.

## Objectives

- Understand the Principle of Least Privilege (PoLP).
- Understand the attack surface of a virtual machine.
- Audit active network ports on a Linux server.
- Configure UFW using a Default Deny policy.
- Allow SSH and HTTP application traffic on port 8080.
- Document security configurations using Markdown.

## Commands Executed

```bash
# Run the Nginx web application
docker run -d --name secure-web-app -p 8080:80 nginx

# Test the web application
curl http://localhost:8080

# Check active listening ports
sudo ss -tuln

# Allow SSH access
sudo ufw allow ssh

# Configure default firewall policies
sudo ufw default deny incoming
sudo ufw default allow outgoing

# Enable the firewall
sudo ufw enable

# Check firewall status
sudo ufw status verbose

# Allow application traffic
sudo ufw allow 8080/tcp

# Display numbered firewall rules
sudo ufw status numbered

# Test the application again
curl http://localhost:8080
```

## Skills Learned

- Deploying an Nginx Docker container.
- Testing a web application using curl.
- Checking active network ports.
- Configuring UFW firewall rules.
- Applying the Default Deny security policy.
- Managing SSH and application access.
- Writing technical documentation in Markdown.
- Organizing a GitHub cloud computing portfolio.
