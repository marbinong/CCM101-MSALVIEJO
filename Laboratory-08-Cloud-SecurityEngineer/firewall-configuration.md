# Firewall Configuration

## Mission 8: The Cloud Security Engineer

This document lists the commands used to configure UFW and secure the Ubuntu server.

## 1. Allow SSH

```bash
sudo ufw allow ssh
```

This allows incoming SSH connections on port 22 so administrators can remotely manage the server.

## 2. Set the Default Deny Policy

```bash
sudo ufw default deny incoming
sudo ufw default allow outgoing
```

The first command blocks incoming connections unless explicitly allowed. The second command permits outgoing connections by default.

## 3. Enable the Firewall

```bash
sudo ufw enable
```

Confirm the prompt if requested.

**Important:** Allowing SSH before enabling UFW helps prevent administrators from losing remote access to the server.

If UFW is enabled before SSH is allowed, incoming SSH connections may be blocked by the default incoming-deny policy, potentially locking out remote administrators.

## 4. Verify the Firewall

```bash
sudo ufw status verbose
```

This displays the firewall status, default policies, and configured rules.

## 5. Allow Port 8080

```bash
sudo ufw allow 8080/tcp
```

This allows incoming TCP traffic on port 8080 for the web application.

## 6. Verify Numbered Rules

```bash
sudo ufw status numbered
```

This displays the firewall rules with numbers so they can be reviewed and managed.

## 7. Test the Web Application

```bash
curl http://localhost:8080
```

A successful response should display the Nginx welcome page HTML.

## Security Best Practices

- Allow only the ports required by the application.
- Allow SSH before enabling the firewall.
- Avoid exposing database ports directly to the public internet.
- Review firewall rules regularly.
- Keep the operating system and applications updated.
- Use strong authentication for administrative access.
