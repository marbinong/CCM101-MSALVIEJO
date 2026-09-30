# Docker Compose Guide

## What Does the `services:` Block Do?

The `services:` block defines the containers that will be created and managed by Docker Compose. In this project, there are two services:

* `database` - uses the MariaDB image.
* `app` - uses the Nextcloud image.

Each service contains its own image, environment variables, and other configuration settings.

## How Does Nextcloud Find the Database?

The Nextcloud container finds the database container through the `MYSQL_HOST` environment variable.

```yaml
- MYSQL_HOST=database
```

The value `database` is the name of the MariaDB service in the Compose file. Docker Compose creates a network for the services, allowing the Nextcloud container to communicate with the database using the service name.

## Docker Run vs Docker Compose

The `docker run` command is normally used to create and start one container at a time. It requires the user to provide the configuration through command-line options.

Docker Compose uses a YAML file to define multiple containers and their configurations. With:

```bash
docker-compose up -d
```

Docker Compose can create and start the whole application stack at once.

## Compose File Used

```yaml
version: '3'

services:

  database:
    image: mariadb:10.6
    environment:
      - MYSQL_ROOT_PASSWORD=cloudnova_root
      - MYSQL_PASSWORD=cloudnova_pass
      - MYSQL_DATABASE=nextcloud_db
      - MYSQL_USER=nextcloud_user

  app:
    image: nextcloud
    ports:
      - 8080:80
    environment:
      - MYSQL_PASSWORD=cloudnova_pass
      - MYSQL_DATABASE=nextcloud_db
      - MYSQL_USER=nextcloud_user
      - MYSQL_HOST=database
```

## Useful Commands

Start the containers:

```bash
docker-compose up -d
```

Check the containers:

```bash
docker-compose ps
```

Stop and remove the containers:

```bash
docker-compose down
```

