# Container Observability Report

## 1. Overview

This report documents the monitoring of the Nginx web server container using Docker logs and real-time container metrics.

## 2. Application Logging

**Command executed:**

```bash
docker logs clientwebsite
```

### HTTP 404 Error Log

Paste the exact log line showing the `404` error below:

```text
[Paste the actual HTTP 404 log line from your terminal here]
```

### Importance of Application Logs

Application logs are important because they show requests, errors, and other events that happen inside an application. They help developers and system administrators identify problems and determine what needs to be fixed.

**Screenshot:** `screenshots/docker-logs.png`

## 3. Real-Time Container Metrics

**Command executed:**

```bash
docker stats
```

### Recorded Metrics

- Container Name: `clientwebsite`
- CPU Usage: [Enter the actual CPU percentage]
- Memory Usage: [Enter the actual memory usage, such as 3.5MiB]
- Network I/O: [Enter the actual received and transmitted values]

Record the values displayed while the container is running.

**Screenshot:** `screenshots/container-metrics.png`

## 4. Analysis

Docker logs provide information about application activity and errors, while Docker stats displays the container's resource consumption. Using both tools helps monitor application behavior and assess the container's performance.

## 5. Conclusion

The monitoring process demonstrates how Docker logs and resource metrics can help assess a containerized application's health. The recorded results provide evidence of the requests handled and the resources consumed by the Nginx container.

