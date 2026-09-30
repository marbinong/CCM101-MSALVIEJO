# Multi-Tier Architecture

## What is a Two-Tier Architecture?

A two-tier architecture is an application structure that separates the application into two main parts: the web/application tier and the database tier. In this laboratory activity, Nextcloud works as the application tier while MariaDB works as the database tier.

## The Web/Application Tier

The web/application tier is responsible for providing the application that users interact with. It handles HTTP requests and displays the Nextcloud web interface. In this activity, the Nextcloud container serves as the web/application tier.

## The Database Tier

The database tier is responsible for storing and managing persistent data. It can store information such as user accounts, credentials, and application metadata. In this activity, MariaDB is used as the database container.

## Why Separate Them?

Separating the web application and database into different containers makes the system easier to manage and maintain. Each container can perform its own role, and changes to one service can be made without directly affecting the other service. It also makes the application easier to scale and deploy.

