# CCM101 Cloud Computing

## Laboratory Activity 1 – Mission 1: Introduction to the Cloud

### Mission Overview

This laboratory activity provides an introduction to the basic skills used in cloud infrastructure. It covers working with a Linux environment, managing files and directories, viewing system information, and building a GitHub portfolio.

---

## Mission Objectives

- Access a Linux environment through KillerCoda.
- Practice navigating and using the Linux operating system.
- Check important system information.
- Manage files and directories using Linux commands.
- Create and organize a GitHub repository.
- Document activities and technical work using Markdown.

---

# Checkpoint 1 – Entering the Cloud

For this checkpoint, I accessed an Ubuntu Linux Playground through KillerCoda. I created a new Linux account named `msalviejo`, set up its Bash shell and home directory, and provided the account with sudo privileges.

### User Information

| Information | Result |
|---|---|
| Current Username | `msalviejo` |
| Current Working Directory | `/home/msalviejo` |
| Hostname | `[Your Hostname]` |

### Commands Used

```bash
sudo adduser msalviejo
sudo usermod -aG sudo msalviejo
su - msalviejo

whoami
pwd
hostname
