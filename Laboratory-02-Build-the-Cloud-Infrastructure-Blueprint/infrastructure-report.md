# Cloud Infrastructure Assessment Report

## Operating System

The Linux server is running:

- Operating System: [INSERT YOUR RESULT]

## Kernel Version

- Kernel Version: [INSERT YOUR RESULT]

## CPU Information

- CPU Model: [INSERT YOUR RESULT]
- Number of CPU Cores: [INSERT YOUR RESULT]

## Memory

- Total RAM: [INSERT YOUR RESULT]

## Storage

- Disk Capacity: [INSERT YOUR RESULT]

## Mounted File Systems

The following file systems are mounted on the server:

[INSERT IMPORTANT RESULTS FROM findmnt]

## Hostname

- Hostname: [INSERT YOUR RESULT]

## IP Address

- IP Address: [INSERT YOUR RESULT]

## Linux Commands Used

The following commands were used to investigate the cloud server:

```bash
cat /etc/os-release
uname -r
lscpu | grep "Model name"
nproc
free -h
df -h
findmnt
hostname
hostname -I
