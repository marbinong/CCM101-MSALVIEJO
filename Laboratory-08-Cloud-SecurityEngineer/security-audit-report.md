# Security Audit Report

## Mission 8: The Cloud Security Engineer

### 1. Principle of Least Privilege (PoLP)

The Principle of Least Privilege means giving users and applications only the permissions they need to perform their tasks. It is important in cloud environments because it reduces the risk of unauthorized access and limits the damage that can happen if an account is compromised.

### 2. Attack Surface

The attack surface refers to all the points where an attacker might try to access or compromise a virtual machine. These include open network ports, running services, applications, and exposed user accounts. Reducing unnecessary services and open ports helps make the server more secure.

### 3. Default Deny Policy

A Default Deny policy blocks incoming network traffic unless a specific rule allows it. This is safer than blocking individual attackers because unknown or unwanted connections are denied automatically instead of relying on a list of known threats.

## Security Audit

### Application Deployment

An Nginx web server was deployed using Docker with the container name `secure-web-app`. The application was mapped to port 8080 on the host.

### Initial Test

The `curl` command was used to check whether the web application responded successfully.

```bash
curl http://localhost:8080
```

### Network Port Audit

The following command was used to check listening network ports:

```bash
sudo ss -tuln
```

### Firewall Configuration

UFW was configured to deny incoming traffic by default and allow outgoing traffic. SSH access was allowed before enabling the firewall, and TCP port 8080 was explicitly allowed for the web application.

### Evidence

Screenshots of the application test, active firewall status, and numbered firewall rules are stored in the `screenshots/` folder.

- `screenshots/vulnerable-app-running.png`
- `screenshots/firewall-activated.png`
- `screenshots/firewall-port-allowed.png`

## Conclusion

The activity demonstrates how a host-based firewall and careful port management can reduce a server's exposure to unwanted network connections. Only necessary services should be accessible, and firewall rules should be reviewed regularly.
