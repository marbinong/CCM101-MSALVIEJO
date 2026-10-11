# Laboratory Activity 7: The Cloud Operations Engineer

## Mission Overview

This laboratory activity focuses on cloud operations, system monitoring, and container observability. It uses the KillerCoda Playground to monitor Linux server resources, deploy an Nginx web server using Docker, generate HTTP requests, and examine application logs and container metrics.

## Objectives

- Monitor CPU, memory, and disk usage using Linux commands.
- Deploy an Nginx web server container using Docker.
- Generate HTTP requests using `curl`.
- Examine application logs using `docker logs`.
- Monitor container CPU and memory usage using `docker stats`.
- Document system performance and observations using Markdown.

## Monitoring Commands Executed

| Command | Purpose |
|---|---|
| `free -h` | Check memory usage |
| `df -h /` | Check root filesystem storage |
| `top` | Monitor active processes and CPU usage |
| `docker run` | Deploy the Nginx container |
| `curl` | Generate HTTP requests |
| `docker logs` | View container application logs |
| `docker stats` | Monitor container resource usage |

## Skills Learned

- Linux system monitoring
- Docker container deployment
- HTTP request testing
- Application log analysis
- Container resource monitoring
- Technical documentation using Markdown

## Repository Structure

```text
Laboratory-07-Cloud-Operations-Engineer/
├── README.md
├── system-baseline-report.md
├── container-observability.md
├── reflection.md
└── screenshots/
    ├── memory-check.png
    ├── disk-check.png
    ├── install-nginx.png
    ├── simulation1.png
    ├── simulation2.png
    ├── docker-logs.png
    └── container-metrics.png
```
