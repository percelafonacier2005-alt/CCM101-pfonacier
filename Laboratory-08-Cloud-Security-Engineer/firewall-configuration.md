# Firewall Configuration

## Allow SSH Access

Command used:

```bash
sudo ufw allow ssh
```

This rule allows SSH connections so administrators can remotely manage the server.

## Configure the Default Deny Policy

Commands used:

```bash
sudo ufw default deny incoming
sudo ufw default allow outgoing
```

The first command blocks incoming traffic by default, while the second allows outgoing traffic from the server.


## Allow Port 8080

Command used:

```bash
sudo ufw allow 8080/tcp
```

This rule allows incoming TCP traffic on port 8080 so users can access the Nginx web application.

To verify the numbered firewall rules, I used:

```bash
sudo ufw status numbered
```

## Importance of Allowing SSH First

If I ran `sudo ufw enable` before `sudo ufw allow ssh`, incoming SSH connections could be blocked by the default-deny policy, potentially locking me out of the remote server.
