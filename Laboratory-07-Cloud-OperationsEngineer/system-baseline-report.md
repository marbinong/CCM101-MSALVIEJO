# System Baseline Report

## 1. Overview

This report documents the initial health check of the Linux server using native Linux monitoring commands. The purpose is to check the server's memory, disk capacity, CPU load, and active processes before deploying a web application.

## 2. Memory Usage

**Command executed:**

```bash
free -h
```

**Results:**

- Total RAM: [Enter the total RAM shown in your terminal]
- Used Memory: [Enter the used memory]
- Available Memory: [Enter the available memory]

**Screenshot:** `screenshots/memory-check.png`

## 3. Disk Storage

**Command executed:**

```bash
df -h /
```

**Results:**

- Total Storage Capacity: [Enter the Size value]
- Used Storage: [Enter the Used value]
- Available Storage: [Enter the Avail value]

**Screenshot:** `screenshots/disk-check.png`

### Why Checking Disk Space Is Important

Checking disk space is important before a massive traffic surge because insufficient storage can prevent applications from writing logs, storing temporary files, and operating properly.

## 4. CPU and Process Monitoring

**Command executed:**

```bash
top
```

The `top` command displays active processes and real-time CPU and memory usage. I observed the changing system metrics to understand the server's current performance.

**Screenshot:** [Add a screenshot if required by your instructor.]

## 5. Conclusion

The system baseline check provides an initial overview of the Linux server's resources. These results can be used to help identify resource limitations during application deployment and monitoring.

