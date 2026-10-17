# Laboratory 08 – The Cloud Security Engineer

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

**1. Allow SSH access**
```bash
sudo ufw allow ssh
```

**2. Set the default-deny incoming policy**
```bash
sudo ufw default deny incoming
```

**3. Allow outgoing traffic**
```bash
sudo ufw default allow outgoing
```

**4. Enable the firewall**
```bash
sudo ufw enable
```

**5. Check firewall status**
```bash
sudo ufw status verbose
```

**6. Allow TCP traffic on port 8080**
```bash
sudo ufw allow 8080/tcp
```

**7. Display numbered firewall rules**
```bash
sudo ufw status numbered
```

**8. Test the web application**
```bash
curl http://localhost:8080
```

## Skills Learned

- Configuring a Linux firewall using UFW.
- Applying the principle of default-deny incoming traffic.
- Allowing only necessary network ports and services.
- Checking firewall status and verifying security rules.
- Testing a web server using curl.
- Documenting technical procedures using Markdown and GitHub.
