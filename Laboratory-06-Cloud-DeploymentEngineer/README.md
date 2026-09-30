# Laboratory 06 - Cloud Deployment Engineer

## Mission Overview

In this laboratory activity, I learned how to deploy a multi-container cloud application using Docker Compose. I deployed Nextcloud together with a MariaDB database container. Docker Compose allowed me to manage both containers using one YAML configuration file.

## Objectives

* Understand multi-tier application architecture.
* Create a `docker-compose.yml` file.
* Use Nano to create and edit configuration files.
* Deploy Nextcloud and MariaDB using Docker Compose.
* Check if the containers are running correctly.
* Access Nextcloud through a web browser.
* Document the deployment process using Markdown.

## Commands Executed

```bash
mkdir nextcloud-deployment
cd nextcloud-deployment
nano docker-compose.yml
docker-compose up -d
docker-compose ps
docker-compose down
```

## Skills Learned

* Creating directories using Linux commands.
* Editing files using Nano.
* Writing YAML configuration files.
* Using Docker Compose.
* Deploying multiple containers.
* Checking container status.
* Accessing a containerized web application.
* Understanding Infrastructure as Code (IaC).
* Documenting cloud deployment procedures using Markdown.

