
---

# Checkpoint 3 — `cloud-components.md`

```markdown
# Cloud Infrastructure Components

## 1. Compute Resources

### Purpose

Compute resources provide the processing power required to run applications, services, and workloads. In cloud computing, compute resources can be provisioned and scaled according to the needs of an organization.

### Importance in Cloud Computing

Compute resources are important because applications require CPU and memory to execute tasks. Cloud platforms allow organizations to obtain computing resources without purchasing and maintaining physical servers.

### KillerCoda Linux Environment

The KillerCoda server provides CPU cores and RAM that allow Linux commands, applications, and other workloads to execute. The CPU and memory observed through `lscpu`, `nproc`, and `free -h` represent the available compute resources.

---

## 2. Storage Resources

### Purpose

Storage resources are used to save operating system files, applications, databases, configurations, and user data.

### Importance in Cloud Computing

Reliable storage allows applications and data to remain available even when computing resources change. Cloud providers offer different storage services depending on performance, capacity, and durability requirements.

### KillerCoda Linux Environment

The Linux environment provides disk storage that can be examined using the `df -h` command. Mounted file systems identified using `findmnt` show how storage is organized and made available to the operating system.

---

## 3. Networking Resources

### Purpose

Networking resources allow computers, applications, and users to communicate with each other.

### Importance in Cloud Computing

Networking enables cloud servers to communicate with users, databases, applications, and other cloud services. It is necessary for accessing applications through the Internet and connecting different infrastructure components.

### KillerCoda Linux Environment

The KillerCoda environment has an IP address that allows the server to communicate over the network. The IP address can be identified using the `hostname -I` command.

---

## 4. Operating System

### Purpose

The operating system manages hardware resources and provides the environment where applications and services run.

### Importance in Cloud Computing

An operating system allows cloud workloads to interact with compute, storage, and networking resources. Linux is widely used in cloud environments because of its flexibility, stability, and strong command-line tools.

### KillerCoda Linux Environment

The KillerCoda server provides a Linux operating system. Commands such as `cat /etc/os-release` and `uname -r` can be used to identify the operating system and kernel version.
