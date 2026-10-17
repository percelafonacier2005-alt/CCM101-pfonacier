# Laboratory 08 – Cloud Security Engineer

## Mission Overview

This laboratory activity focuses on securing a web application using the UFW (Uncomplicated Firewall) on an Ubuntu server. The goal is to reduce security risks by blocking incoming traffic by default and allowing only the required services.

## Objectives

- Understand the Principle of Least Privilege and attack surface.
- Learn how to audit and manage network access.
- Configure UFW with a default-deny incoming policy.
- Allow SSH access for remote administration.
- Allow TCP traffic on port 8080 for the Nginx web application.
- Verify firewall rules and test the web application using curl.


## Commands Executed 
Commands Executed

# Start the Nginx container
docker run -d --name secure-web-app -p 8080:80 nginx

# Permit SSH connections
sudo ufw allow ssh

# Set the default firewall policies
sudo ufw default deny incoming
sudo ufw default allow outgoing

# Turn on the firewall
sudo ufw enable

# View the firewall configuration
sudo ufw status verbose

# Permit web traffic on TCP port 8080
sudo ufw allow 8080/tcp

# View the firewall rules with numbers
sudo ufw status numbered

# Check the web server response
curl http://localhost:8080
